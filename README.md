# 📋 Projeto com HTML, JavaScript e Tailwind CSS v4

Este é um projeto simples de front-end utilizando apenas **HTML**, **JavaScript** e **Tailwind CSS v4**, com configuração manual via PostCSS.

## 💠 Estrutura do Projeto

```
/meu-projeto/
├── index.html
├── main.js
├── tailwind.config.js
├── postcss.config.js
├── package.json
└── src/
    └── styles.css
```

## 🚀 Tecnologias Utilizadas

- [Tailwind CSS v4](https://tailwindcss.com/)
- HTML5
- JavaScript (ES6)
- PostCSS

## 📆 Instalação

1. Clone este repositório:

```bash
git clone https://github.com/seu-usuario/seu-repo.git
cd seu-repo
```

2. Instale as dependências:

```bash
npm install
```

3. Compile o CSS com Tailwind:

```bash
npx tailwindcss -i ./src/styles.css -o ./dist/styles.css --watch
```

> Isso gerará o arquivo `styles.css` com as classes utilitárias do Tailwind CSS.

## 🌈 Exemplo de uso

No `index.html`, importe o CSS gerado:

```html
<link href="./dist/styles.css" rel="stylesheet" />
```

E use as classes utilitárias no HTML normalmente:

```html
<h1 class="text-2xl text-h-red-200 font-bold">Olá Tailwind 4!</h1>
```

## 🎨 Cores Personalizadas

O arquivo `tailwind.config.js` está configurado com as seguintes cores personalizadas usando a diretiva `@theme` (CSS variables):

```js
// Exemplo dentro do tailwind.config.js
theme: {
  extend: {
    colors: {
      'h-red-100': 'var(--h-red-100)',
      'h-gray-50': 'var(--h-gray-50)',
      'h-white-400': 'var(--h-white-400)',
      // e assim por diante...
    }
  }
}
```

E as variáveis podem ser definidas dentro de `styles.css` ou globalmente com `@theme {}`:

```css
@theme {
  --h-red-100: #FFCCCC;
  --h-gray-50: #CCCCCC;
  --h-white-400: #FFFFFF;
}
```

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

Feito com 💙 por [Kened Felix](https://github.com/k3n3dfelix)

