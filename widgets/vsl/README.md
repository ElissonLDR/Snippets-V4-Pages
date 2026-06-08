# VSL YouTube com Formulário

Snippet de VSL para V4 Pages com vídeo do YouTube, formulário de desbloqueio, timer de oferta e bloqueio de avanço no player.

## Arquivo

- `vsl-youtube-com-formulario.html` — snippet completo para colar em um bloco HTML da página.

## Placeholders (substituir antes de publicar)

| Placeholder | Onde | Exemplo |
|---|---|---|
| `ID_DO_VIDEO_YOUTUBE` | URL do embed ao desbloquear | `W8-R1uX-u_c` |
| `TEMPO_LIBERACAO_SEGUNDOS` | Variável `liberarEm` | `585` (9:45) ou `660` (11:00) |
| `URL_DO_WEBHOOK` | `fetch()` após envio do form | `https://seu-webhook.com/...` |
| `LINK_DO_BOTAO_CTA` | Link do botão após o timer | `https://sua-lp.com/oferta` |
| `TEXTO_DO_BOTAO_CTA` | Texto do botão CTA | `Garantir minha vaga` |
| `TITULO_DO_VIDEO` | Atributo `title` do iframe | `VSL - Nome do produto` |

## Funcionalidades

- Formulário bloqueia o vídeo até preencher nome e WhatsApp
- Autoplay só após desbloquear (iframe vazio antes)
- Bloqueio de cliques nas laterais, topo e fundo (40%) — só pause no centro
- Timer oculto até desbloquear; ao zerar exibe CTA + "Oferta liberada!"
- Seta pulsante no rodapé do vídeo quando a oferta libera
- Scroll suave centraliza o vídeo após desbloquear
- Máscara e validação de WhatsApp BR
- Proteção contra embed duplicado na mesma página

## Uso no V4 Pages

1. Copie o conteúdo de `vsl-youtube-com-formulario.html`
2. Substitua todos os placeholders
3. Cole em **um único** bloco HTML da página (não duplicar o snippet)
4. Teste no celular: formulário, autoplay, timer e botão CTA

## Timer

O valor é em **segundos**. Exemplos:

- `300` → 5:00
- `585` → 9:45
- `660` → 11:00
