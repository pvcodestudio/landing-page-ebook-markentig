# MarketUp — Landing Page Premium de Marketing Digital

Landing page de alta conversão desenvolvida para captação de leads através da distribuição de um ebook gratuito de marketing digital. Construída com padrões profissionais de engenharia front-end, design editorial SaaS moderno, código 100% humanizado e zero dependências pesadas.

---

## 🎯 Objetivo do Projeto

Oferecer uma experiência de navegação rápida, fluida e confiável para o usuário final, apresentando os benefícios do ebook *"The Digital Marketing Playbook"* e convertendo visitantes em leads qualificados com conformidade à LGPD.

---

## 🎨 Design System & Identidade Visual

- **Direção de Arte:** Modern SaaS, Dark UI editorial sofisticado.
- **Paleta de Cores:**
  - Fundo principal: `#060D1B`
  - Fundo secundário: `#0B1729`
  - Superfícies (Cards): `#101E34` / `#17263D`
  - Bordas: `#263954`
  - Textos: `#F7F9FC` (Principal) | `#A6B3C8` (Secundário) | `#72839D` (Mudo)
  - Destaques (Accents): Laranja (`#FF914D`), Azul Ciano (`#26C5FF`), Roxo (`#8A45FF`), Verde Menta (`#35E3B8`), Rosa (`#FF557D`)
- **Tipografia:** Família `Inter` carregada com otimização (`preconnect` e `font-display: swap`).
- **Efeitos:** Glassmorphism com desfoque de fundo (`backdrop-filter: blur(16px)`), sombras suaves e iluminação sutil.
- **Mockup 3D:** O ebook na seção Hero foi construído inteiramente com **HTML e CSS 3D moderno** (`transform-style: preserve-3d`, perspectiva realística e sombra projetada), sem necessidade de imagens pesadas ou bibliotecas externas.

---

## 📁 Estrutura de Arquivos

```text
testegemini/
├── index.html                  # Estrutura semântica, SEO, OpenGraph e acessibilidade
├── assets/
│   ├── css/
│   │   ├── style.css           # Tokens de design, estilos base e componentes
│   │   └── responsive.css      # Media queries (Desktop, Tablet e Mobile)
│   ├── js/
│   │   └── main.js             # Menu mobile, validação de form, accordion e animações
│   └── images/                 # Diretório para ativos visuais e fotos
└── README.md                   # Documentação completa do projeto
```

---

## ✨ Funcionalidades e Diferenciais

1. **Código Humanizado e Separação Estrita de Responsabilidades:**
   - Separação total entre marcação e apresentação: **zero estilos inline ou blocos `<style>` no HTML**.
   - Variáveis CSS (design tokens) reutilizáveis centralizadas em `style.css`.
   - Comentários contextualizados e explicativos, sem excessos ou linhas desnecessárias.
   - Nomes de classes semânticos seguindo boas práticas de BEM/Utility.

2. **Acessibilidade Completa (WCAG 2.2 AA):**
   - Link de salto para o conteúdo principal (`.skip-link`).
   - Gerenciamento de atributos ARIA (`aria-expanded`, `aria-controls`, `aria-label`, `aria-live`).
   - Foco visível com alto contraste para navegação por teclado (`:focus-visible`).
   - Respeito à preferência do sistema operacional por redução de movimentos (`prefers-reduced-motion`).

3. **SEO Técnico Avançado:**
   - Meta tags OpenGraph e Twitter Cards completas.
   - Marcação semântica Schema.org em formato JSON-LD (`Organization`, `WebPage`, `FAQPage`).
   - Estrutura hierárquica de títulos (`h1`, `h2`, `h3`) consistente.

4. **Componentes Interativos:**
   - **Cabeçalho Fixo (Sticky Header):** Suporte a menu hambúrguer interativo para mobile.
   - **Hero Section com Ebook 3D:** Ebook com animação de flutuação suave e card analítico complementar.
   - **Módulos do Conteúdo:** Apresentação clara em linhas horizontais responsivas.
   - **Formulário com Validação em Tempo Real:** Valida campos no `blur` e no `submit`, exibe spinners de carregamento e fornece feedback acessível.
   - **FAQ Accordion:** Tira-dúvidas interativo com fechamento inteligente de itens anteriores.

---

## 🚀 Como Executar Localmente

Como o projeto foi construído em tecnologia web nativa (HTML5, CSS3, JavaScript ES6+), não é obrigatório nenhum processo de build ou compilação.

### Opção 1: Abrir diretamente no navegador
Basta dar um duplo clique no arquivo `index.html` ou arrastá-lo para qualquer navegador moderno (Chrome, Edge, Firefox, Safari).

### Opção 2: Servidor local simples (Recomendado)
Para testar a experiência completa de requisições de rede:

- **Com Node.js (npx):**
  ```bash
  npx serve .
  ```
- **Com Python 3:**
  ```bash
  python -m http.server 8000
  ```
  Acesse `http://localhost:8000`.

- **Com a extensão Live Server (VS Code):**
  Clique com o botão direito em `index.html` e selecione **"Open with Live Server"**.

---

## 🔌 Integração de Backend (Endpoint `/api/leads`)

O formulário em `assets/js/main.js` já está preparado para enviar requisições `POST` no formato JSON:

```json
{
  "name": "Nome do Lead",
  "email": "lead@exemplo.com",
  "marketingConsent": true,
  "createdAt": "2026-10-23T16:55:00.000Z"
}
```

Caso o projeto seja executado em um ambiente sem servidor ativo, o script detecta automaticamente a ausência da rota e simula uma resposta com sucesso para demonstração visual imediata.

---

## 📄 Licença e Direitos

Projeto desenvolvido para a marca **MarketUp**. Todos os direitos reservados.
