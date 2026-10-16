# 📋 Documentação Técnica e Funcional do Site Atual — Cerealista Pansani

Esta documentação foi elaborada para servir como especificação completa de migração e modernização do frontend da **Cerealista Pansani**. Ela contém todas as regras de negócio, dados institucionais, catálogo de produtos, estrutura de arquivos, diagnóstico de problemas e um prompt pronto para ser enviado à IA que desenvolverá o novo frontend.

---

## 1. Visão Geral do Negócio

- **Nome da Empresa:** Cerealista Pansani
- **Segmento:** Agropecuária, Pet Shop e Empório Caipira / Produtos Coloniais
- **Tempo de Mercado:** 37 anos de tradição
- **Slogan / Proposta de Valor:** *"Tradição e qualidade. Direto do produtor para sua casa!"*
- **Diferenciais:** Tradição familiar, atendimento próximo e acolhedor, produtos a granel (rações para criação e pet, cereais e variedades) e produtos artesanais autênticos da roça (ovos caipiras, cachaças, mel e café).

---

## 2. Inventário de Arquivos e Assets Existentes

| Arquivo | Descrição / Conteúdo | Dimensões / Características |
| :--- | :--- | :--- |
| `index.html` | Arquivo único contendo HTML, CSS em `<style>` e JS embutido. | Estrutura SPA com navegação por exibição/ocultação de `<section>`. |
| `logo.png` | Logotipo com estética azul giz/desenho rústico: *"Cerealista Pansani — RAÇÕES E GRÃOS"*. | Fundo xadrez claro / efeito caderno, estilo rústico tradicional. |
| `about-image.jpg` | Foto real do balcão de atendimento com o mascote (gata tricolor), garrafas artesanais e sacos de ração. | Foto vertical de alta autenticidade e conexão emocional com o cliente. |
| `Menu.jpg` | Montagem/colagem de fotos dos produtos dividida em categorias. | Contém fotos de ovos, cachaça, mel, café, rações variadas, granel e milho. |
| **Repositório Git** | `https://github.com/luisfa27/cerealistapansani.git` | Configurado para hospedagem no GitHub Pages (`/cerealistapansani/`). |

---

## 3. Conteúdo Completo e Textos Atuais por Seção

### 3.1. Cabeçalho (Header / Navbar)
- **Marca:** Ícone de pata (`fa-paw`) + texto "Cerealista Pansani" (ou logotipo).
- **Links de Navegação:**
  - `Home` (`#home`)
  - `Sobre` (`#sobre`)
  - `Produtos` (`#produtos`)
  - `Contato` (`#contato`)
- **Menu Mobile:** Botão hambúrguer com toggle lateral/dropdown.

### 3.2. Seção Hero (Início)
- **Logo de boas-vindas:** Imagem do logotipo centralizada.
- **Título principal (H1):** `Direto do produtor para você!`
- **Subtítulo:** `Qualidade, variedade e o melhor atendimento. Encontre tudo que você precisa para seus animais em um só lugar.`
- **Botão de Ação (CTA):** `Conheça nossos produtos` (aponta para a seção `#produtos`).

### 3.3. Seção Sobre Nós
- **Título da Seção (H2):** `Nossa História, Sua Confiança`
- **Subtítulo:** `Tradição e modernidade caminhando juntas para oferecer sempre o melhor para você.`
- **Imagem de Apoio:** Foto do balcão e da loja (`about-image.jpg`).
- **Título do Bloco:** `Bem-vindo à Cerealista Pansani!`
- **Texto Institucional:**
  > *"A Cerealista Pansani tem o compromisso, há 37 anos, de oferecer os melhores produtos para o campo e para seus animais de estimação. Com uma tradição de qualidade e bom atendimento, buscamos sempre a satisfação de nossos clientes."*
  >
  > *"Nossa equipe está sempre pronta para ajudar você a encontrar o que precisa, seja para sua criação de animais de grande porte, para seus pets ou para sua horta e jardim. Venha nos visitar e descubra a diferença que a paixão pelo que fazemos pode oferecer."*

### 3.4. Seção Produtos
- **Título da Seção (H2):** `Nossos Produtos`
- **Subtítulo:** `Soluções completas em rações, cereais e produtos naturais com a qualidade que você já conhece.`
- **Categorias atuais (Cards com ícones):**
  1. **Linha Pet** (Ícone: `fa-dog`):
     - Rações para Gatos e Cachorros (Premium a Superpremium)
     - Rações para aves (pássaros)
     - Rações para coelhos
  2. **Linha Agro** (Ícone: `fa-wheat-awn`):
     - Rações para equinos, suínos e bovinos
     - Rações para peixes e aves
     - Milho, soja e outros cereais, por saca ou a granel
  3. **Naturais do Produtor** (Ícone: `fa-leaf`):
     - Mel puro e derivados
     - Ovos caipiras frescos
     - Café artesanal da região
     - Cachaças artesanais
- **Painel Visual Existente:** Imagem estática `Menu.jpg` com os produtos fotografados individualmente (Ovo caipira, Cachaça artesanal, Mel artesanal, Café artesanal, Rações variadas, Rações a granel, Milho).

### 3.5. Seção Contato & Localização
- **Título da Seção (H2):** `Entre em Contato`
- **Subtítulo:** `Estamos prontos para te atender! Fale conosco pelo WhatsApp e venha nos visitar.`
- **Dados Oficiais de Atendimento:**
  - **WhatsApp / Telefone:** `(16) 99359-6161`
    - Link direto: `https://wa.me/5516993596161`
  - **Horário de Funcionamento:**
    - Segunda a Sexta-feira: `07:00 – 17:30`
    - Sábado: `07:00 – 12:00`
    - Domingo: Fechado
  - **Endereço Físico:**
    - `R. Joaquim Leôncio Coelho, 120 - Jardim Conceição Leite, Franca - SP, 14405-362`
  - **Mapa Integrado:** Iframe do Google Maps apontando para as coordenadas do endereço.

### 3.6. Rodapé (Footer)
- **Copyright:** `© 2025 Cerealista Pansani. Todos os direitos reservados.`
- **Links Sociais:** Facebook, Instagram e WhatsApp.

---

## 4. Stack Atual e Implementação Técnica

- **Linguagens:** HTML5 puro + CSS3 embutido na tag `<style>` + JavaScript Vanilla embutido em `<script>`.
- **Tipografia:** Google Fonts — `'Nunito', sans-serif` (pesos 400, 700, 800).
- **Biblioteca de Ícones:** Font Awesome 6.4.0 via CDN (`cdnjs`).
- **Paleta de Cores Atual:**
  - Primária: `#6B4F4F` (Marrom rústico)
  - Secundária: `#4CAF50` (Verde agro)
  - Destaque/Acento: `#FF9800` (Laranja pet)
  - Fundo: `#FDFCF8` (Off-white amendoado)
  - Texto: `#333333`
  - WhatsApp: `#25D366` / `#128C7E`
- **Mecanismo de Roteamento:** SPA estático rudimentar onde o JavaScript manipula `section.style.display = 'none'` e `'block'` ao clicar nos links da barra de navegação.

---

## 5. Diagnóstico de Problemas e Oportunidades de Modernização

| Ponto Fraco Atual | Impacto Negativo | Oportunidade de Melhoria no Novo Frontend |
| :--- | :--- | :--- |
| **Imagem estática `Menu.jpg`** | Texto preso na imagem, não indexável no Google, ilegível em telas menores e visual amador. | Transformar em cards/grid interativo com fotos individuais, badges, busca e botão "Pedir pelo WhatsApp". |
| **Navegação com `display: none`** | Seções ficam ocultas por padrão; impede rolagem suave contínua e quebra deep links / SEO. | Navegação fluida tipo *One-Page Landing Page* com rolagem suave (`scroll-behavior: smooth`) e links âncora reais. |
| **Ausência de Botão Flutuante** | O cliente só vê o WhatsApp se rolar até a seção de contato ou rodapé. | Adicionar botão flutuante pulsante de WhatsApp no canto inferior direito, com mensagem pré-formatada. |
| **Design visual rústico antigo** | Layout quadrado sem microinterações, profundidade ou sensação premium moderna. | Design moderno com estética acolhedora ("Modern Rustic / Agro Chic"), cards com sombras suaves, blur glassmorphism no header e microanimações. |
| **SEO e Metadados Básicos** | Falta Open Graph (preview no WhatsApp/Instagram), Twitter Card e schema `LocalBusiness`. | Adicionar meta tags completas e Schema JSON-LD de negócio local para ranquear em buscas de Franca e região. |
| **Chamadas para Ação (CTAs)** | Poucos pontos de conversão direta para o WhatsApp ao longo da navegação. | CTAs contextuais em cada categoria de produto ("Consultar preço da saca", "Pedir no Zap"). |

---

## 6. Prompt de Instrução Pronto para a Nova IA de Frontend

Copie e cole as instruções abaixo diretamente para a IA que irá construir a nova versão:

```markdown
Você é um desenvolvedor frontend e designer de UI/UX sênior. 
Preciso que você modernize completamente o site institucional da "Cerealista Pansani", uma empresa tradicional com 37 anos de história no ramo Agro, Pet e Produtos Artesanais/Coloniais localizada em Franca - SP.

### Objetivo
Construir uma Landing Page moderna, responsiva, com visual profissional e acolhedor (estilo Agro Chic / Modern Rustic), focada em alta conversão via WhatsApp e excelente experiência tanto em smartphones quanto em desktops.

### Dados da Empresa e Conteúdos Obrigatórios:
1. **Identidade:** Cerealista Pansani (37 anos de tradição).
2. **Slogan:** "Direto do produtor para você! Qualidade, variedade e o melhor atendimento. Encontre tudo que você precisa para seus animais em um só lugar."
3. **Contato & Atendimento:**
   - WhatsApp / Telefone: (16) 99359-6161 (Link direto: https://wa.me/5516993596161?text=Ol%C3%A1!%20Gostaria%20de%20informa%C3%A7%C3%B5es%20sobre%20os%20produtos%20da%20Cerealista%20Pansani)
   - Horários: Seg a Sex: 07:00 – 17:30 | Sáb: 07:00 – 12:00
   - Endereço: R. Joaquim Leôncio Coelho, 120 - Jardim Conceição Leite, Franca - SP, 14405-362
4. **Seções da Landing Page:**
   - **Header Fixo / Sticky:** Logotipo, menu de navegação suave (Home, Sobre, Produtos, Galeria, Contato), botão de destaque "Falar no WhatsApp" e menu hambúrguer para mobile.
   - **Hero Section:** Headline forte, selo de "37 Anos de Tradição", botões de ação ("Ver Produtos" e "Chamar no WhatsApp"), e elementos visuais de impacto.
   - **Sobre Nós:** História da loja, valores de confiança familiar, destaque para o atendimento humanizado e espaço para a foto da loja (about-image.jpg).
   - **Catálogo Interativo de Produtos (Substituindo o antigo Menu.jpg por componentes interativos):**
     * Categorias:
       a) Linha Pet (Rações Premium/Superpremium para cães e gatos, rações para aves/pássaros, coelhos).
       b) Linha Agro (Rações para equinos, suínos, bovinos, peixes e aves; cereais como milho e soja a granel e por saca).
       c) Empório e Naturais do Produtor (Mel puro e derivados, ovos caipiras frescos, café artesanal da região, cachaças artesanais).
     * Cada item ou card deve conter: badge de categoria, ícone/foto, descrição rápida e botão direto de "Pedir pelo WhatsApp".
   - **Diferenciais / Por que escolher a Pansani:** Cards com ícones destacando: Grãos e Rações a Granel, Preço Direto do Produtor, Produtos Artesanais Selecionados e Tradição de 37 Anos.
   - **Localização e Contato:** Cards organizados com horário, endereço com link para Google Maps / Waze, botão de chamada telefônica/WhatsApp e Iframe interativo do Google Maps.
   - **Botão Flutuante do WhatsApp:** Fixado no canto inferior com animação de pulso suave e tooltip "Fale Conosco".
   - **Rodapé:** Links rápidos, dados institucionais, copyright e links de redes sociais.

### Requisitos de Design e Código:
- **Tecnologias:** HTML5 semântico, CSS3 moderno (Variáveis CSS, Flexbox, CSS Grid) e JavaScript limpo (sem dependências pesadas, ou framework se solicitado).
- **Tipografia:** Moderna e legível (ex: Google Fonts 'Plus Jakarta Sans', 'Inter' ou 'Outfit').
- **Paleta de Cores Recomendada:**
  - Primária: Verde folha/campo refinado (ex: `#1E4D2B` ou `#2D6A4F`)
  - Acento: Âmbar/Laranja mel quente (ex: `#E76F51` ou `#F4A261`)
  - Neutros: Branco puro, Off-white aconchegante (`#FBFBF8`), Cinza escuro para tipografia (`#1F2937`)
  - Suporte WhatsApp: `#25D366`
- **Mobile First e Responsividade:** Perfeito em telas pequenas (360px+) até monitores ultrawide.
- **Acessibilidade & SEO:** Alt em imagens, tags semânticas, meta tags Open Graph e JSON-LD LocalBusiness.
```
