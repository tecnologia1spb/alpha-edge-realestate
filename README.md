# 🏢 Alpha Edge Real Estate - Dashboard Financeiro Inteligente

![Version](https://img.shields.io/badge/version-1.2.0-blue.svg)
![React](https://img.shields.io/badge/React-18.3.1-blue.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-blue.svg)
![Tremor UI](https://img.shields.io/badge/Tremor_UI-3.18.7-purple.svg)
![Supabase](https://img.shields.io/badge/Supabase-2.52.1-green.svg)
![License](https://img.shields.io/badge/license-Private-red.svg)

> **Dashboard financeiro inteligente para análise de portfólio imobiliário de Shopping Centers com IA integrada**

## 🎯 Visão Geral

O **Alpha Edge Real Estate** é uma aplicação moderna de dashboard financeiro desenvolvida especificamente para análise de portfólio imobiliário de Shopping Centers. Integra inteligência artificial para insights automáticos, análise preditiva de inadimplência e otimização de performance financeira.

### 📊 Características Principais

- **Dashboard Inteligente**: 5 módulos especializados (Overview, Financeiro, Inadimplência, Orçamento, Analytics)
- **IA Integrada**: Framework AVA da Ant Design para insights automáticos
- **Dados Reais**: Integração com Supabase contendo 15k+ registros financeiros
- **Performance Otimizada**: Web Workers para cálculos não-bloqueantes
- **Localização BR**: 100% em português brasileiro

## 🚀 Tecnologias Utilizadas

### Core Stack
- **React 18.3.1** - Interface moderna e reativa
- **TypeScript 5.5.3** - Tipagem robusta e desenvolvimento seguro
- **Vite 5.4.1** - Build tool otimizado para desenvolvimento

### UI/UX
- **Tremor UI 3.18.7** - Biblioteca de componentes para dashboards profissionais
- **Tailwind CSS 3.4.11** - Framework CSS utilitário
- **Lucide React** - Ícones modernos e consistentes
- **Date-fns** - Formatação de datas localizada (pt-BR)

### Inteligência Artificial
- **@antv/ava 3.4.1** - Framework para insights automáticos
- **@antv/ava-react 3.3.2** - Componentes React para análise visual

### Backend & Dados
- **Supabase 2.52.1** - Backend-as-a-Service com PostgreSQL
- **TanStack Query 5.56.2** - Gerenciamento de estado do servidor
- **React Hook Form + Zod** - Formulários tipados com validação

### Qualidade de Código
- **ESLint 9.9.0** - Análise de código com regras customizadas
- **TypeScript ESLint** - Regras específicas para TypeScript
- **Husky + lint-staged** - Pre-commit hooks para qualidade

## 📈 Dados em Produção

O sistema integra com dados reais do **Shopping Park Botucatu**:

| Tabela | Registros | Descrição |
|--------|-----------|-----------|
| **faturamento** | 3,513 | Receitas por locatário e shopping |
| **inadimplencia** | 10,791 | Análise de risco e inadimplência |
| **movimentacoes_financeiras** | 1,030 | Transações (~R$ 28M em volume) |
| **Pagamento_Empreendedor** | 1,131 | Pagamentos de fornecedores |

## 🖥️ Módulos do Dashboard

### 📊 1. Overview Dashboard
- KPIs consolidados do portfólio
- Performance vs benchmark de mercado
- Composição e diversificação
- Insights financeiros automáticos com IA

### 💰 2. Financial Dashboard  
- Análise detalhada de receitas e NOI
- Fluxo de caixa e despesas operacionais
- Indicadores financeiros avançados
- Comparativos mensais e anuais

### ⚠️ 3. Inadimplência Dashboard
- Taxa de inadimplência em tempo real
- Sistema de scoring de risco com IA
- Top 10 maiores inadimplentes
- Análise preditiva e recomendações

### 🎯 4. Orçamento Dashboard
- Controle orçamentário por categoria
- Execução vs planejado
- Análise de fornecedores
- Identificação de oportunidades de economia

### 🧠 5. Analytics Dashboard
- Modelos preditivos com Machine Learning
- Análise de risco-retorno
- Simulações Monte Carlo
- Network analysis do portfólio

## 🛠️ Instalação e Desenvolvimento

### Pré-requisitos
- Node.js 18+ 
- npm ou yarn
- Git

### Clone e Configuração
```bash
# Clone o repositório
git clone https://github.com/tecnologia1spb/alpha-edge-realestate.git
cd alpha-edge-realestate

# Instale as dependências
npm install

# Configure as variáveis de ambiente
cp .env.example .env.local
# Adicione suas credenciais do Supabase
```

### Scripts Disponíveis

```bash
# Desenvolvimento
npm run dev              # Servidor de desenvolvimento (porta 8080)
npm run build            # Build para produção  
npm run preview          # Preview do build

# Qualidade de Código
npm run lint             # Análise ESLint
npm run lint:fix         # Correção automática
npm run validate:imports # Validação de imports de ícones
npm run validate:all     # Validação completa
npm run check:dashboard  # Validação + build (CI/CD)
```

## 🔧 Configuração

### Variáveis de Ambiente
```env
# Supabase (dados públicos - sem autenticação)
VITE_SUPABASE_URL=https://vdhxtlnadjejyyydmlit.supabase.co
VITE_SUPABASE_ANON_KEY=sua_chave_anonima_supabase

# Desenvolvimento
NODE_ENV=development
```

### Estrutura de Pastas
```
src/
├── components/           # Componentes React
│   ├── Dashboard/       # Módulos principais do dashboard
│   ├── ui/              # Componentes UI reutilizáveis
│   ├── charts/          # Gráficos especializados
│   └── Layout/          # Componentes de layout
├── hooks/               # Custom hooks React
├── lib/                 # Utilitários e helpers
├── workers/             # Web Workers para performance
├── integrations/        # Integrações (Supabase, etc.)
└── pages/               # Componentes de página
```

## 🧠 Inteligência Artificial

### Framework AVA Integration
- **Detecção Automática**: Identifica tendências, anomalias e correlações
- **Insights Contextuais**: Recomendações específicas para real estate
- **Análise Preditiva**: Previsões de inadimplência e performance
- **Processamento Não-bloqueante**: Web Workers mantêm UI responsiva

### Tipos de Insights Gerados
- 📈 **Tendências**: Crescimento/decrescimento em métricas
- 🚨 **Anomalias**: Valores fora do padrão esperado  
- 🔗 **Correlações**: Relações entre variáveis financeiras
- 🎯 **Previsões**: Pontos de mudança detectados pela IA
- ⚠️ **Alertas**: Padrões de risco identificados

## 📊 Performance e Otimização

### Web Workers
- Cálculos financeiros pesados executados em background
- Interface sempre responsiva durante processamento
- Cache inteligente para resultados frequentes

### Otimizações Implementadas
- **Lazy Loading**: Componentes carregados sob demanda
- **React Query**: Cache de 5 minutos para dados do servidor
- **Bundle Splitting**: Chunks otimizados para loading
- **Tree Shaking**: Remoção de código não utilizado

## 🔒 Segurança e Dados

### Modelo de Dados
- **Público**: Dashboard acessa apenas dados não-sensíveis
- **Sem Autenticação**: Supabase configurado com chave anônima
- **Read-Only**: Sistema não modifica dados de produção

### Validação e Qualidade
- **Zod Schemas**: Validação de dados em runtime
- **TypeScript**: Tipagem estática para prevenção de erros
- **ESLint Rules**: 209 regras de qualidade implementadas
- **Pre-commit Hooks**: Validação automática antes de commits

## 📋 Roadmap

### 🎯 Próximas Funcionalidades
- [ ] **Módulo Portfolio**: Otimização MPT (Modern Portfolio Theory)
- [ ] **Monte Carlo**: Simulações avançadas de risco
- [ ] **Geo Intelligence**: Analytics espacial dos shopping centers
- [ ] **Alpha Signals**: Detecção automática de oportunidades
- [ ] **Export/Import**: Relatórios PDF e integração Excel
- [ ] **Alertas Real-time**: Notificações proativas
- [ ] **Mobile App**: Versão nativa para iOS/Android

### 🔧 Melhorias Técnicas
- [ ] **GraphQL**: Migração do REST para GraphQL
- [ ] **Micro-frontends**: Arquitetura modular
- [ ] **PWA**: Progressive Web App capabilities
- [ ] **E2E Testing**: Testes automatizados com Playwright
- [ ] **Docker**: Containerização para deployment
- [ ] **CI/CD**: Pipeline automatizado GitHub Actions

## 🤝 Contribuição

### Padrões de Desenvolvimento
1. **Commits Convencionais**: feat, fix, chore, docs
2. **Branch Strategy**: GitFlow (main, develop, feature/*)
3. **Code Review**: Pull requests obrigatórios
4. **Qualidade**: 100% TypeScript, 0 ESLint errors

### Como Contribuir
```bash
# 1. Fork do repositório
# 2. Criar branch feature
git checkout -b feature/nova-funcionalidade

# 3. Desenvolvimento com qualidade
npm run validate:all

# 4. Commit seguindo convenções
git commit -m \"feat: implementar nova funcionalidade\"

# 5. Push e Pull Request
git push origin feature/nova-funcionalidade
```

## 📜 Histórico de Versões

### v1.2.0 (28/01/2025) - Limpeza e Otimização
- ✅ 209 erros ESLint corrigidos
- ✅ Imports não utilizados removidos
- ✅ Tipagem TypeScript melhorada
- ✅ Sistema de validação de qualidade implementado

### v1.1.0 (28/01/2025) - Correções e Melhorias
- ✅ Sistema holístico de prevenção de erros
- ✅ Otimização de ESLint com regras específicas
- ✅ Repositório GitHub configurado

### v1.0.0 (25/01/2025) - Release Inicial
- ✅ Dashboards completos implementados
- ✅ Integração Supabase funcional
- ✅ Framework AVA para IA
- ✅ Localização portuguesa brasileira

## 📞 Contato e Suporte

- **Repositório**: [GitHub](https://github.com/tecnologia1spb/alpha-edge-realestate)
- **Issues**: [Bug Reports & Feature Requests](https://github.com/tecnologia1spb/alpha-edge-realestate/issues)
- **Discussions**: [Discussões Técnicas](https://github.com/tecnologia1spb/alpha-edge-realestate/discussions)

## 📄 Licença

Este projeto é **privado** e propriedade da **tecnologia1spb**. Todos os direitos reservados.

---

**🤖 Generated with [Claude Code](https://claude.ai/code)**

*Dashboard financeiro inteligente para o futuro do Real Estate brasileiro* 🇧🇷