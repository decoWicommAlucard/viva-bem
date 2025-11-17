# Viva Bem - Agenda de Saúde Preventiva

Um site informativo sobre saúde preventiva que apresenta os principais exames de rotina organizados por faixa etária, com seções específicas para prevenção feminina e masculina.

## 📋 Sobre o Projeto

O **Viva Bem** é uma plataforma educativa que visa conscientizar sobre a importância dos exames preventivos de saúde. O site apresenta informações detalhadas sobre:

- Exames de rotina por faixa etária (15, 20, 25, 30, 40 e 50 anos)
- Prevenção específica para mulheres
- Prevenção específica para homens
- Alertas importantes sobre autoexames e vacinação
- Links úteis para recursos de saúde

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica e acessível
- **SCSS/SASS** - Pré-processador CSS para estilização modular
- **Browser Sync** - Servidor de desenvolvimento com live reload
- **npm** - Gerenciador de pacotes

## 📁 Estrutura de Arquivos

```
viva-bem/
├── index.html                 # Página principal
├── package.json              # Dependências e scripts
├── src/
│   ├── css/                  # CSS compilado (gerado automaticamente)
│   │   └── styles.css
│   ├── img/                  # Imagens do projeto
│   │   ├── logo-*.png        # Logos (desktop/mobile/footer)
│   │   ├── banner-hero.png   # Banner principal
│   │   ├── icon-*.svg        # Ícones dos alertas
│   │   └── image-card-*-prevent*.png  # Imagens dos cards
│   └── scss/                 # Código-fonte SCSS
│       ├── styles.scss       # Arquivo principal (importa todos os módulos)
│       ├── base/             # Estilos base
│       │   ├── _base.scss    # Estilos globais e tipografia
│       │   ├── _mixins.scss  # Mixins reutilizáveis
│       │   ├── _reset.scss   # Reset CSS
│       │   ├── _tokens.scss  # Variáveis (cores, fontes, espaçamentos)
│       │   └── _utils.scss   # Classes utilitárias
│       └── layout/           # Estilos dos componentes
│           ├── _alerts.scss  # Seção de alertas
│           ├── _footer.scss  # Rodapé
│           ├── _header.scss  # Cabeçalho
│           ├── _hero.scss    # Seção hero
│           ├── _importance.scss  # Seção de importância
│           └── _prevention.scss  # Seção de prevenção
```

## 🚀 Como Começar

### Pré-requisitos

- Node.js (versão 14 ou superior)
- npm (geralmente vem com Node.js)

### Instalação

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd viva-bem
```

2. Instale as dependências:
```bash
npm install
```

## 📜 Scripts Disponíveis

### Desenvolvimento

Inicia o servidor de desenvolvimento com live reload e compilação automática do SCSS:

```bash
npm run dev
```

Este comando executa em paralelo:
- `sass:watch` - Compila SCSS automaticamente quando há mudanças
- `serve` - Inicia o Browser Sync na porta 3000

### Compilação de Produção

Gera o CSS minificado para produção:

```bash
npm run build
```

### Scripts Individuais

- `npm run sass:watch` - Compila SCSS em modo watch (desenvolvimento)
- `npm run serve` - Inicia apenas o servidor Browser Sync

## 🎨 Sistema de Design

### Tokens de Design

O projeto utiliza um sistema de tokens centralizado em `src/scss/base/_tokens.scss`:

#### Cores
- **Primária**: `#04031c` (brand-dark)
- **Secundária**: `#1173d4`
- **Gradientes**: Definidos para diferentes seções (hero, botões, títulos)

#### Tipografia
- **Fontes**: 
  - Inter (h3, h4, h5)
  - Roboto (h1, h2, p, span)
- **Tamanhos**: Sistema em rem (base 16px)
- **Pesos**: 400 (regular), 500 (medium), 600 (semibold), 700 (bold)

#### Espaçamentos e Dimensões
- Container máximo: `1120px`
- Raios de borda: 6px a 50px
- Altura de botões: `44px`

### Estrutura SCSS

O projeto segue a metodologia **BEM** (Block Element Modifier) para nomenclatura de classes:

```scss
.block {
  &__element {
    // Estilos do elemento
  }
  
  &--modifier {
    // Estilos do modificador
  }
}
```

## 📱 Seções do Site

### 1. Header
Cabeçalho com logo e navegação principal, com design em gradiente e bordas arredondadas.

### 2. Hero
Seção principal com título, descrição e botões de ação (CTA).

### 3. Importância
Apresenta três cards explicando a importância dos exames preventivos:
- Detecção Precoce
- Cuidado Familiar
- Qualidade de Vida

### 4. Prevenção Feminina
Cards informativos organizados por faixa etária (15, 20, 25, 30, 40, 50 anos) com os exames recomendados.

### 5. Prevenção Masculina
Similar à seção feminina, com recomendações específicas para homens.

### 6. Alertas
Quatro cards de alerta sobre:
- Autoexame das Mamas
- Autoexame dos Testículos
- Vacinas em Dia
- Saúde Mental

### 7. Footer
Rodapé com logo, links úteis (Ministério da Saúde, INCA, SUS) e informações de contato.

## ♿ Acessibilidade

O projeto foi desenvolvido com foco em acessibilidade:

- Uso de elementos semânticos HTML5
- Atributos ARIA apropriados (`aria-label`, `aria-labelledby`, `role`)
- Textos alternativos em todas as imagens
- Estrutura de navegação clara
- Contraste adequado de cores

## 🌐 Navegadores Suportados

- Chrome (últimas 2 versões)
- Firefox (últimas 2 versões)
- Safari (últimas 2 versões)
- Edge (últimas 2 versões)

## 📝 Licença

ISC

## 👥 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📞 Contato e Recursos

- **Disque Saúde**: 136
- **Email**: sac@saude.gov.br
- **Emergência**: SAMU 192

### Links Úteis
- [Ministério da Saúde](https://www.gov.br/saude/)
- [INCA - Instituto Nacional do Câncer](https://www.inca.gov.br/)
- [SUS - Sistema Único de Saúde](https://www.gov.br/saude/pt-br/assuntos/setor-saude/sus)

---

**Nota**: As informações apresentadas neste site são baseadas em diretrizes médicas nacionais e internacionais. Sempre consulte um profissional de saúde para orientações personalizadas.

