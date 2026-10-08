# SEMENTE · Cofres Desafio

Mini loja de uma página: catálogo dos 13 modelos, envio para as 11 províncias de Moçambique e encomenda enviada pelo WhatsApp.

Site estático: só `index.html` e a pasta `img/`. Não precisa de build.

## Antes de publicar

No fim do `index.html`, no bloco **CONFIGURAÇÃO DA LOJA**:

| Campo | O que pôr |
| --- | --- |
| `WHATSAPP` | Número com indicativo, só dígitos, ex.: `25884XXXXXXX` |
| `PRECOS` | Preço em MT por tamanho: `C` compacto, `P` pequeno, `M` médio, `G` grande (os valores atuais são exemplos) |

## Publicar no GitHub Pages

1. *Settings → Pages*
2. *Source*: **Deploy from a branch**, branch `main`, pasta `/ (root)`
3. O site fica em https://mohvi.github.io/semente-cofres/

GitHub Pages em repositórios privados exige um plano pago; num plano grátis o repositório tem de ser público.

## Ver localmente

```bash
python3 -m http.server 8000
# abrir http://localhost:8000
```
