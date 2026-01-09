# 🍎 MacBook Landing Page

> Landing page interativa com modelo 3D do MacBook Pro usando React Three Fiber e GSAP

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=three.js&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)

## 📋 Sobre o Projeto

Landing page moderna e interativa que apresenta o MacBook Pro com um modelo 3D totalmente customizável. O usuário pode interagir com o modelo, alterando cores e explorando o produto em 360 graus com animações suaves.

### ✨ Funcionalidades

- 🎨 **Customização de Cores** - Altere a cor do MacBook em tempo real
- 🔄 **Rotação 360°** - Explore o modelo em todos os ângulos
- 📱 **Design Responsivo** - Funciona perfeitamente em desktop e mobile
- ⚡ **Animações Fluidas** - Transições suaves usando GSAP
- 🖼️ **Modelo 3D Realista** - MacBook Pro M3 16" 2024 em alta qualidade

## 🚀 Tecnologias Utilizadas

- **React** - Biblioteca JavaScript para interfaces
- **Vite** - Build tool moderna e rápida
- **Three.js** - Biblioteca para gráficos 3D
- **React Three Fiber** - Renderer React para Three.js
- **React Three Drei** - Helpers úteis para R3F
- **GSAP** - Biblioteca de animações
- **Zustand** - Gerenciamento de estado
- **Tailwind CSS** - Framework CSS utility-first

## 📦 Instalação

### Pré-requisitos

- Node.js (versão 16 ou superior)
- npm ou yarn

### Passo a passo

1. **Clone o repositório**
```bash
git clone https://github.com/edneyzl/macbook_landingpage.git
cd macbook_landingpage
```

2. **Instale as dependências**
```bash
npm install
```

3. **Inicie o servidor de desenvolvimento**
```bash
npm run dev
```

4. **Abra no navegador**
```
http://localhost:5173
```

## 🛠️ Scripts Disponíveis

```bash
# Iniciar servidor de desenvolvimento
npm run dev

# Build para produção
npm run build

# Preview da build de produção
npm run preview

# Lint do código
npm run lint
```

## 📁 Estrutura do Projeto

```
macbook_landingpage/
├── public/
│   ├── models/           # Modelos 3D (.glb)
│   ├── screen.png        # Textura da tela
│   └── vite.svg
├── src/
│   ├── components/       # Componentes React
│   │   ├── MacbookModel14.jsx
│   │   └── ...
│   ├── constants/        # Constantes do projeto
│   │   └── index.js
│   ├── store/           # Gerenciamento de estado (Zustand)
│   │   └── index.js
│   ├── App.jsx          # Componente principal
│   ├── App.css          # Estilos principais
│   └── main.jsx         # Ponto de entrada
├── index.html
├── package.json
└── vite.config.js
```

## 🎨 Customização

### Adicionar novas cores

Edite o arquivo `src/constants/index.js`:

```javascript
export const colors = [
  { name: 'Prateado', color: '#C0C0C0' },
  { name: 'Space Gray', color: '#53565A' },
  { name: 'Dourado', color: '#FFD700' },
  // Adicione sua cor aqui
  { name: 'Nova Cor', color: '#HEX_CODE' }
]
```

### Modificar o modelo 3D

1. Substitua o arquivo em `public/models/macbook-14-transformed.glb`
2. Ajuste os materiais em `MacbookModel14.jsx`

## 🌐 Deploy

### GitHub Pages

1. Configure o `vite.config.js`:
```javascript
base: '/macbook_landingpage/'
```

2. Instale gh-pages:
```bash
npm install --save-dev gh-pages
```

3. Adicione no `package.json`:
```json
"homepage": "https://edneyzl.github.io/macbook_landingpage",
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d dist"
}
```

4. Faça o deploy:
```bash
npm run deploy
```

### Vercel (Recomendado)

```bash
npm i -g vercel
vercel
```

## 🐛 Problemas Conhecidos

- [ ] Modelo 3D pode demorar para carregar em conexões lentas
- [ ] Performance reduzida em dispositivos móveis antigos

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:

1. Fazer um fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abrir um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Edney ZL**

- GitHub: [@edneyzl](https://github.com/edneyzl)

## 🙏 Créditos

- Modelo 3D: [MacBook Pro M3 16" 2024](https://sketchfab.com/3d-models/macbook-pro-m3-16-inch-2024-8e34fc2b303144f78490007d91ff57c4) por [jackbaeten](https://sketchfab.com/jackbaeten)
- Licença do modelo: [CC-BY-4.0](http://creativecommons.org/licenses/by/4.0/)

## 📸 Screenshots

<img src="/images/Hero.png" alt="Hero" />
<img src="/images/Product.png" alt="Product" />
<img src="/images/Features.png" alt="Features" />
<img src="/images/Highlights.png" alt="Highlights" />
<img src="/images/Footer1.png" alt="Footer" />
<img src="/images/Footer2.png" alt="Footer" />

## 🔗 Links Úteis

- [Documentação React Three Fiber](https://docs.pmnd.rs/react-three-fiber)
- [Three.js Docs](https://threejs.org/docs/)
- [GSAP Docs](https://greensock.com/docs/)
- [Zustand Docs](https://zustand-demo.pmnd.rs/)

---

⭐ Se você gostou deste projeto, deixe uma estrela no repositório!
