# Biblioteca Digital UniFECAF

Projeto acadêmico de Design Web desenvolvido com **HTML5 e CSS3**, sem frameworks e sem JavaScript.

## Como visualizar

1. Extraia a pasta `biblioteca-unifecaf`.
2. Abra `index.html` em um navegador atualizado.
3. Para conferir o layout em smartphone, redimensione a janela para até 700 px de largura ou use a visualização responsiva do navegador.

## Estrutura

```text
biblioteca-unifecaf/
├── index.html
├── css/
│   └── style.css
├── assets/
│   └── imagens/
├── capturas/
│   ├── desktop-view.png
│   ├── mobile-view.png
│   ├── desktop.png
│   └── mobile.png
└── README.md
```

A pasta `assets/imagens/` está preparada para imagens locais adicionais. As ilustrações principais são SVG inline no HTML e as capas demonstrativas são compostas em CSS. A pasta `capturas/` contém prévias desktop/mobile e capturas completas de rolagem.

## Como o código está organizado

### `index.html`

- `header`: marca tipográfica, navegação desktop e menu expansível em mobile.
- `hero`: mensagem principal, chamadas para ação e ilustração vetorial.
- `quick-stats`: indicadores em faixa azul.
- `about-section`: apresentação da biblioteca e benefícios.
- `quote-band`: faixa editorial de destaque.
- `books-section`: seis sugestões de leitura com links para a página oficial.
- `access-section`: biblioteca física, bibliotecas digitais e repositório acadêmico.
- `contact-section` e `footer`: canais institucionais e encerramento da página.

### `css/style.css`

- As variáveis de cor, raios e largura máxima ficam no início do arquivo (`:root`).
- Grid e Flexbox organizam os blocos e os cards.
- A media query de 980 px ajusta o layout para telas intermediárias.
- A media query de 700 px reorganiza o conteúdo para smartphone e ativa o menu mobile.
- `:focus-visible` destaca o elemento selecionado pelo teclado e `prefers-reduced-motion` reduz as transições quando solicitado pelo sistema.

Para trocar cores, edite as variáveis dentro de `:root`. Para alterar títulos e parágrafos, edite os textos correspondentes no `index.html`. Os links de consulta podem ser atualizados sem mexer no layout.

## Decisões e limites do protótipo

- A navegação usa âncoras internas e links para a página institucional da biblioteca.
- O menu mobile usa o elemento nativo `<details>`, sem JavaScript.
- Os seis livros são sugestões editoriais e não representam confirmação de estoque.
- O bloco chamado "As unidades" no protótipo foi adaptado para três caminhos de acesso: biblioteca física, bibliotecas digitais e repositório acadêmico. O briefing não informa três endereços físicos distintos.
- O nome da instituição aparece como identificação do projeto acadêmico. A marca tipográfica é uma representação de interface, não um arquivo oficial de logotipo.
- Esta versão não contém login, banco de dados, busca integrada, empréstimo ou reserva. Os botões direcionam aos canais públicos institucionais.

## Fontes institucionais e técnicas

- UniFECAF, Biblioteca: https://www.unifecaf.com.br/biblioteca
- MDN, elementos HTML: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element
- MDN, media queries: https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_media_queries/Using_media_queries
- W3C, WCAG 2.2: https://www.w3.org/TR/WCAG22/
- Material Design: https://m2.material.io/
