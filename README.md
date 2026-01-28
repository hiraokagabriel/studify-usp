# Studify USP 🎓

> Aplicativo completo de gerenciamento de estudos para medicina na USP

## 🚀 Funcionalidades

### 📚 Sistema de Flashcards
- Criação e edição de flashcards
- Sistema de repetição espaçada (Spaced Repetition)
- Categorização por matérias
- Estatísticas de progresso
- Modo de revisão com algoritmo inteligente

### 📅 Gerenciador de Horários
- Grade horária semanal completa
- Cadastro de aulas com professor, sala e horário
- Lembretes automáticos
- Visualização por dia/semana

### ⏰ Sistema de Prazos
- Gerenciamento de entregas e trabalhos
- Priorização por urgência
- Notificações de proximidade
- Descrição detalhada de cada entrega
- Status de conclusão

### 🏷️ Sistema de Tags
- Tags personalizadas para organização
- Filtros por tags
- Cores customizáveis
- Associação com qualquer item (flashcard, tarefa, etc.)

### 📋 Quadro Kanban
- Colunas customizáveis (A Fazer, Em Progresso, Concluído)
- Drag and drop intuitivo
- Cards com descrição, tags e prazos
- Visualização de progresso

### 📊 Dashboard de Estudos
- Estatísticas de estudo diário/semanal/mensal
- Gráficos de progresso
- Horas estudadas por matéria
- Metas e objetivos

### 🎯 Recursos Adicionais
- Modo escuro/claro
- Exportação de dados
- Backup automático
- Busca global
- Filtros avançados

## 🛠️ Tecnologias

- **Frontend**: React 18 + TypeScript
- **Desktop**: Tauri 2.0
- **Estilização**: TailwindCSS
- **Ícones**: Lucide React
- **Drag & Drop**: dnd-kit
- **Build**: Vite
- **Persistência**: Local Storage + Tauri FS

## 📦 Instalação

### Pré-requisitos

- Node.js 18+
- Rust 1.70+
- Windows: Microsoft Visual Studio C++ Build Tools
- macOS: Xcode Command Line Tools
- Linux: Dependências do sistema (ver docs Tauri)

### Passo a passo

```bash
# Clone o repositório
git clone https://github.com/hiraokagabriel/studify-usp.git
cd studify-usp

# Instale as dependências
npm install

# Execute em modo desenvolvimento
npm run tauri dev

# Build para produção
npm run tauri build
```

## 🎮 Uso

### Desenvolvimento
```bash
npm run dev          # Apenas frontend (navegador)
npm run tauri dev    # App completo desktop
```

### Build
```bash
npm run build        # Build frontend
npm run tauri build  # Build app desktop
```

## 📁 Estrutura do Projeto

```
studify-usp/
├── src/                    # Código fonte React
│   ├── components/         # Componentes React
│   │   ├── Flashcards/    # Sistema de flashcards
│   │   ├── Schedule/      # Horários de aula
│   │   ├── Deadlines/     # Prazos e entregas
│   │   ├── Kanban/        # Quadro Kanban
│   │   ├── Tags/          # Sistema de tags
│   │   └── Dashboard/     # Dashboard principal
│   ├── hooks/             # Custom React hooks
│   ├── types/             # TypeScript types
│   ├── utils/             # Funções utilitárias
│   ├── App.tsx            # Componente principal
│   └── main.tsx           # Entry point
├── src-tauri/             # Código Rust do Tauri
│   ├── src/
│   │   └── main.rs        # Backend Tauri
│   ├── Cargo.toml         # Dependências Rust
│   └── tauri.conf.json    # Configuração Tauri
├── public/                # Assets estáticos
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

## 🎨 Interface

O aplicativo possui uma interface moderna e intuitiva com:
- Navegação por abas lateral
- Tema escuro/claro adaptável
- Responsivo e otimizado
- Atalhos de teclado
- Busca global (Ctrl+K)

## 💾 Armazenamento

Os dados são salvos localmente usando:
- LocalStorage para configurações rápidas
- Tauri FS API para persistência robusta
- Backup automático diário

## 🔒 Privacidade

Todos os seus dados ficam **100% locais** no seu computador. Nenhuma informação é enviada para servidores externos.

## 📝 Licença

MIT License - Livre para uso pessoal e distribuição

## 🤝 Contribuindo

Este é um projeto pessoal, mas contribuições são bem-vindas!

1. Fork o projeto
2. Crie uma branch (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

## 📧 Contato

Para dúvidas ou sugestões, abra uma issue no GitHub.

---

**Desenvolvido com ❤️ para estudantes de medicina da USP**

Bons estudos! 🚀📚