# SEMENTE · Cofres Desafio

Mini loja de uma página: catálogo dos 13 modelos, envio para as 11 províncias de Moçambique e encomenda enviada pelo WhatsApp.

Site estático: só `index.html` e a pasta `img/`. Não precisa de build.

## Antes de publicar

No fim do `index.html`, no bloco **CONFIGURAÇÃO DA LOJA**:

| Campo | O que pôr |
| --- | --- |
| `WHATSAPP` | Número com indicativo, só dígitos, ex.: `25884XXXXXXX` |
| `PRECOS` | Preço em MT por tamanho: `C` compacto, `P` pequeno, `M` médio, `G` grande (os valores atuais são exemplos) |

## Alojamento

O site está no **Vercel** (projeto ligado a este repositório: cada push para `main` publica automaticamente) com o domínio **semente.store**.

DNS na TuaSolução (nameservers `ns1/ns2.tuasolucao.com`):

| Tipo | Nome | Valor |
| --- | --- | --- |
| A | `@` | `216.198.79.1` (Vercel) |
| CNAME | `www` | `b8af26c6600da7e2.vercel-dns-017.com.` (Vercel) |

O email continua no servidor da TuaSolução: **não alterar** `mail`, `smtp`, `pop`, `ftp`, o MX nem o TXT do SPF.

## Publicar no GitHub Pages (alternativa)

1. *Settings → Pages*
2. *Source*: **Deploy from a branch**, branch `main`, pasta `/ (root)`
3. (Opcional) O site principal está no Vercel em https://semente.store/

GitHub Pages em repositórios privados exige um plano pago; num plano grátis o repositório tem de ser público.

## Ver localmente

```bash
python3 -m http.server 8000
# abrir http://localhost:8000
```
