# Site — Dra. Raquel Amaral · Ortodontia

Página única, estática e autocontida (`index.html`, com CSS e JS embutidos). Não há etapa de build: basta publicar a pasta em qualquer hospedagem estática (Netlify, Vercel, GitHub Pages, servidor próprio).

Prévia local:

```bash
cd site-dra-raquel
python3 -m http.server 8765
# abra http://localhost:8765
```

## Fotografias pendentes

A logo oficial (monograma RA) está em `assets/logo-raquel-amaral.*`. Nenhuma foto original foi entregue para o projeto. Por isso, cada área fotográfica usa uma arte vinho e rosé com facetas lapidadas, marcada no HTML com `data-photo-slot`. Ao lado de cada uma há um comentário com o `<img>` pronto para substituí-la. Coloque os arquivos em `assets/`.

| Slot | Onde | Arquivo sugerido | Formato |
|---|---|---|---|
| `abertura` | metade direita da primeira tela | `assets/raquel-cadeira.jpg` | vertical, ≥ 1200 × 1600, rosto no terço superior |
| `recepcao` | faixa de largura total (quadro central) | `assets/recepcao.jpg` | 4:5 ou horizontal amplo |
| `retrato` | apresentação da dentista | `assets/raquel-retrato.jpg` | vertical 4:5, ≥ 900 × 1125 |
| `localizacao` | seção “O consultório fica no Paraíso” | `assets/recepcao.jpg` | vertical 4:5 |

Recomendações: exporte em JPEG/WebP com qualidade 75–80 e no máximo ~250 KB por arquivo, mantenha `width`/`height` no `<img>` e use `loading="lazy"` em todas as imagens, exceto a da abertura. Ao trocar o retrato, substitua o `<picture>` da logo dentro de `.portrait`.

## Links configurados

- WhatsApp (agendamento): `wa.me/5511984093430`, com a mensagem de avaliação
- WhatsApp (tratamentos): mensagem “Olá! Vi os tratamentos no site da Dra. Raquel e gostaria de tirar uma dúvida.”
- Rota: Google Maps até Praça Oswaldo Cruz, 47, Paraíso, São Paulo, SP, 04004-070
- Telefone `tel:+5511984093430`, e-mail, Instagram e Facebook
