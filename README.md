# Vectra Mídia — Site institucional (redesign "Design 3")

Landing page da **Vectra Mídia** com o visual "Design 3": fundo escuro com tom azulado, um brilho roxo/azul de nebulosa no topo, botões brancos em formato de pílula e cartões com bordas finas.

Todo o conteúdo do site anterior foi mantido (textos, fotos, prints, links do Instagram e seções).

---

## Estrutura de arquivos

```
index.html              → a página (todo o conteúdo)
assets/css/style.css    → o visual (cores, fontes, espaçamentos)
assets/js/main.js       → o funcionamento (menu, vídeos, prints, WhatsApp, cookies)
assets/js/config.js     → as configurações (número do WhatsApp, mensagens, e-mail)
assets/images/          → fotos, logo e prints
data/testimonials.json  → dados de depoimentos (referência)
vercel.json             → configuração da hospedagem na Vercel
```

---

## Como trocar o número do WhatsApp

Abra `assets/js/config.js` e troque o número (55 + DDD + número, só dígitos):

```javascript
whatsappNumber: "5511999999999",
```

Todos os botões do site (topo, serviços, depoimentos, rodapé e o botão verde flutuante) passam a usar o novo número automaticamente. Cada botão já manda uma mensagem pronta diferente (por exemplo, o botão de "Tráfego Pago" já abre o WhatsApp com "quero saber mais sobre Tráfego Pago").

---

## Paleta do Design 3

| Uso | Cor |
|---|---|
| Fundo da página | `#1f232e` |
| Cartões | `#17191e` |
| Caixas mais escuras | `#0c0f19` / `#060913` |
| Texto principal | `#f2f6fa` |
| Texto secundário | `#858b98` |
| Brilho da marca | gradiente `#3245ff → #b845ed` |
| Detalhes (etiquetas e ícones) | menta `#4bf3c8`, azul `#54b9ff`, violeta `#acafff`, âmbar `#ffd493` |

Fontes (Google Fonts): **Space Grotesk** (títulos), **Inter** (textos), **JetBrains Mono** (etiquetas).

---

## Como publicar na Vercel

1. Substitua os arquivos do repositório no GitHub por estes (mantendo a mesma estrutura de pastas).
2. A Vercel publica sozinha a cada atualização do GitHub. Não precisa configurar nada.
