// Crie uma logomarca personalizada em SVG com os seguintes detalhes:
// - Forma principal: Um hexágono com bordas arredondadas
// - Cores: Gradiente radial começando em #00114f (azul escuro) e terminando em #0fba99 (verde água)
// - Texto: "CM Soluções Gráficas", posicionado no centro com fonte Montserrat, peso bold, cor branca
// - Tamanho da fonte: 24px
// - Inclua uma pequena sombra embaixo do texto para destaque
// - Adicione um ícone de uma engrenagem estilizada no canto inferior direito, com 30% da opacidade e 50px de largura
// - O arquivo SVG deve ter um tamanho de 500x500px

const logoSVG = `
<svg width="500" height="500" xmlns="http://www.w3.org/2000/svg">
  <!-- Hexágono com gradiente -->
  <defs>
    <radialGradient id="grad1" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" style="stop-color:#00114f;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#0fba99;stop-opacity:1" />
    </radialGradient>
  </defs>
  <polygon points="250,25 475,150 475,350 250,475 25,350 25,150"
    fill="url(#grad1)" stroke="none" rx="20" ry="20"/>

  <!-- Texto -->
  <text x="50%" y="50%" dominant-baseline="middle" text-anchor="middle"
    font-family="Montserrat" font-size="24" font-weight="bold" fill="#ffffff"
    style="text-shadow: 2px 2px 4px rgba(0,0,0,0.3);">
    CM Soluções Gráficas
  </text>

  <!-- Ícone de engrenagem -->
  <g opacity="0.3" transform="translate(400, 400)">
    <circle cx="0" cy="0" r="25" fill="#ffffff"/>
    <rect x="-15" y="-5" width="30" height="10" fill="#00114f" />
    <rect x="-5" y="-15" width="10" height="30" fill="#00114f" />
  </g>
</svg>
`;

console.log(logoSVG);
