# 🎨 CSS Border-Radius Showcase

Bem-vindo ao **CSS Border-Radius Showcase**! Este é um projeto simples, mas visualmente informativo, criado para demonstrar as diversas maneiras de utilizar a propriedade `border-radius` do CSS. Ele serve como um guia prático e visual para desenvolvedores front-end, desde iniciantes até os mais experientes, que desejam explorar as possibilidades de arredondamento de bordas em seus projetos.

## 🚀 Demo

Visualize o projeto em ação aqui: **[[Link para a Live Demo](https://nexuscleo-commits.github.io/border-radius/)]**

---

## ✨ Funcionalidades

- **Exemplos Visuais:** Cards interativos que mostram o efeito de diferentes valores e sintaxes da propriedade `border-radius`.
- **Snippets de Código:** Cada exemplo visual é acompanhado do respectivo código CSS, pronto para ser copiado e utilizado.
- **Design Responsivo:** A página se adapta a diferentes tamanhos de tela, utilizando CSS Grid Layout para uma visualização otimizada em desktops, tablets e celulares.
- **Animação de Fundo:** Um fundo dinâmico e sutil com gradientes radiais animados (`aurora effect`) para uma experiência visual mais agradável e moderna.

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído utilizando apenas tecnologias web fundamentais, demonstrando o poder do CSS moderno.

- **HTML5:** Para a estrutura semântica do conteúdo.
- **CSS3:** Para toda a estilização, layout, animações e, claro, os exemplos de `border-radius`.

---

## 📂 Estrutura do Projeto

```
BorderRadius/
├── 📄 index.html   # Arquivo principal com a estrutura dos cards
└── 🎨 styles.css   # Folha de estilos com todo o design e lógica visual
```

---

## 🔧 Como Executar Localmente

Para visualizar o projeto em sua máquina local, siga estes passos simples:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/nexuscleo-commits/BorderRadius/archive/refs/heads/main.zip
   ```

2. **Navegue até o diretório do projeto:**
   ```bash
   cd BorderRadius
   ```

3. **Abra o arquivo `index.html`** no seu navegador de preferência. E pronto!

---

## 💡 Análise do Código CSS (`styles.css`)

O arquivo `styles.css` contém algumas técnicas interessantes:

### Animação de Fundo (Aurora)

O efeito de fundo é criado com um pseudo-elemento `::before` no `body`. Três gradientes radiais são posicionados e animados para criar um efeito de luzes dançantes e suaves.

```css
body::before {
    content: "";
    position: fixed;
    background-image: 
        radial-gradient(circle at 25% 25%, #5500ff 0%, transparent 40%),
        radial-gradient(circle at 75% 25%, #ff007f 0%, transparent 40%),
        radial-gradient(circle at 50% 75%, #00e5ff 0%, transparent 40%);
    filter: blur(100px);
    z-index: -1;
    animation: aurora 15s linear infinite;
}

@keyframes aurora {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}
```

### Layout Responsivo com Grid

O container principal dos cards (`.div-container`) utiliza `display: grid` com `repeat(auto-fit, minmax(350px, 1fr))` para criar um layout que se ajusta automaticamente ao número de colunas, dependendo do espaço disponível na tela.

---

## 🤝 Contribuições

Contribuições são sempre bem-vindas! Se você tiver ideias para novos exemplos de `border-radius` ou melhorias no código, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

## 📄 Desenvolvido por Cleomar

&copy;NexusCleo 2025. Todos os direitos reservados.

