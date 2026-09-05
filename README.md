# Icafé — Landing Page

Página de vendas do café **Icafé (café natural da roça)**, feita apenas com
**HTML5 + CSS3** (sem JavaScript e sem frameworks).

## Conteúdo do projeto

```
landing-icafe/
├── index.html    # página principal (estrutura semântica e acessível)
├── styles.css    # todo o visual e a responsividade
├── README.md     # este arquivo
└── img/          # imagens de exemplo (SVG) — substitua por fotos reais
    ├── logo-icafe.svg
    ├── hero-cafe.svg
    ├── prod-*.svg     (6 imagens dos cards de produto)
    └── gal-*.svg      (6 imagens da galeria)
```

## Como visualizar

Abra o arquivo `index.html` em qualquer navegador (dê dois cliques no arquivo
ou arraste para a janela do navegador).

## Seções da página

| Seção          | Âncora        | Descrição                                      |
| -------------- | ------------- | ---------------------------------------------- |
| Início (hero)  | `#inicio`     | Apresentação do produto e botão de compra      |
| Benefícios     | `#beneficios` | 3 benefícios do café                           |
| Produtos       | `#produtos`   | 6 cards com preço e botão de pedido            |
| Galeria        | `#galeria`    | Imagens com legenda                            |
| Sobre          | `#sobre`      | O que é, para quem é e diferenciais            |
| Chamada        | `#cta`        | Destaque antes do contato                      |
| Contato        | `#contato`    | Formulário + e-mail, telefone e endereço       |

## Como editar

1. **Textos** — troque o conteúdo entre as tags `h1`, `h2`, `h3`, `p` e `li`
   no `index.html`. Há comentários indicando cada seção.
2. **Preços** — procure por `class="preco"` no `index.html` e edite o valor.
3. **Imagens** — substitua os arquivos da pasta `img/` pelas suas fotos
   (mantendo os nomes ou atualizando o `src`) e revise o texto `alt` de cada
   `img` para descrever a foto.
4. **Contato** — procure `mailto:`, `tel:` e `wa.me/` no `index.html` e no
   rodapé e troque pelos seus dados.
5. **Redes sociais e links legais** — procure `href="#"` nos blocos comentados
   e coloque os endereços reais.

### Formulário de contato

O formulário usa a validação nativa do navegador (`required`, `type="email"`),
sem JavaScript. Para **receber as mensagens**, adicione o destino de envio no
atributo `action` do formulário, por exemplo:

```html
<form id="formulario-contato" name="formulario-contato" action="https://formspree.io/f/SEU-CODIGO" method="post">
```

Serviços gratuitos que funcionam bem: Formspree, Getform, FormSubmit ou o
backend da sua preferência.

## Acessibilidade e responsividade

- HTML semântico (`header`, `nav`, `main`, `section`, `article`, `figure`,
  `address`, `footer`) e apenas um `h1`.
- Link "Pular para o conteúdo principal", foco visível e navegação total por
  teclado.
- Textos alternativos (`alt`) descritivos nas imagens.
- Contraste adequado (texto/fundo) e mensagens que não dependem só de cor.
- `prefers-reduced-motion` respeitado (sem animações para quem prefere menos
  movimento).
- Layout responsivo: 1 coluna no celular, 2 no tablet e 3 no desktop (cards
  de produto); menu empilhado em telas pequenas.
- Botões com área de toque confortável (mín. 44 px) e conteúdo legível com
  zoom de até 200%.
