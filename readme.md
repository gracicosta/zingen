# Zingen 🎤
 
Landing page de um aplicativo de karaokê que usa Inteligência Artificial para remover a voz original das músicas e avaliar a performance de quem canta.
 
Projeto desenvolvido com foco em **HTML semântico**, **CSS moderno** e **layout responsivo** (mobile, tablet e desktop).
 
## 🔗 Demonstração
 
https://gracicosta.github.io/zingen/
 
## ✨ Funcionalidades da página
 
- **Hero** com chamada principal e botões de conversão
- **Conheça o app** explicando o diferencial da IA
- **Funcionalidades** em grid assimétrico com mockups das telas
- **Planos e preços** com destaque visual para o plano Premium
- **Download** com botões para App Store e Play Store
- **Footer** com navegação secundária e ícones sociais com hover animado
## 🛠️ Tecnologias
 
- HTML5 semântico
- CSS3 puro, utilizando:
  - Custom Properties (design tokens de cor, tipografia e espaçamento)
  - CSS Nesting nativo
  - Grid e Flexbox
  - Media queries com range syntax (`width >= 80rem`)
  - Gradientes com `background-clip: text`
- Classes utilitárias próprias (`.container`, `.even-columns`, `.py-xl`, `.gap-1`…)
- Fonte [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts
## 📁 Estrutura de pastas
 
```
.
├── index.html
├── assets/
│   ├── icons/          # SVGs de ícones, redes sociais e badges das lojas
│   └── imagens/        # Logo, mockups, backgrounds e ilustrações
└── styles/
    ├── style.css       # Arquivo principal (só imports)
    ├── global.css      # Reset, variáveis e tipografia base
    ├── utility.css     # Classes utilitárias e breakpoints
    ├── buttons.css
    ├── social.css
    ├── header.css
    ├── hero.css
    ├── sections.css
    ├── about.css
    ├── cards.css
    ├── features.css
    ├── pricing.css
    ├── download.css
    └── footer.css
```
 
O `style.css` centraliza todos os imports. O `features.css` é carregado apenas em telas grandes:
 
```css
@import url(features.css) (width >= 80rem);
```
 
## 📱 Responsividade
 
A página foi construída em **mobile first**, com três breakpoints principais:
 
| Faixa | Comportamento |
|---|---|
| `< 40rem` | Layout em coluna única, elementos `.desktop-only` ocultos |
| `40rem – 80rem` | Versão tablet, container de 60rem |
| `>= 80rem` | Container de 80rem, grid de funcionalidades, tipografia ampliada |
 
## 🚀 Como rodar
 
```bash
git clone https://github.com/seu-usuario/zingen.git
cd zingen
```
 
Depois é só abrir o `index.html` no navegador ou usar a extensão **Live Server** do VS Code.
 
## 📝 Licença
 
Projeto de estudo, livre para uso e modificação.