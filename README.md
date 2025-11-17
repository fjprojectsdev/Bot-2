# iMavyBot - WhatsApp Bot

Bot avançado para WhatsApp com sistema anti-spam, comandos administrativos e agendamento automático.

## 🚀 Funcionalidades

- **Sistema Anti-Spam**: Detecção automática de links e palavras proibidas
- **Sistema de Strikes**: 3 strikes = expulsão automática
- **Comandos Administrativos**: Fechar/abrir grupo, banir membros, fixar mensagens
- **Agendamento**: Abertura/fechamento automático do grupo
- **Blacklist Personalizada**: Adicionar/remover termos e links bloqueados
- **Notificações**: Alertas automáticos para administradores
- **Boas-vindas**: Mensagem automática para novos membros

## 📋 Pré-requisitos

- Node.js 16+
- NPM ou Yarn
- Conta WhatsApp

## 🛠️ Instalação

1. Clone o repositório:
```bash
git clone https://github.com/fjprojectsdev/Bot-2.git
cd Bot-2
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
```bash
cp .env.example .env
```

4. Edite o arquivo `.env` com suas chaves de API:
- `HUGGING_FACE_API`: Sua chave da Hugging Face
- `GROQ_API_KEY`: Sua chave do Groq
- `OPENROUTER_API_KEY`: Sua chave do OpenRouter

## 🚀 Uso

1. Inicie o bot:
```bash
npm start
```

2. Escaneie o QR code que aparecerá no terminal com seu WhatsApp

3. Configure os grupos permitidos usando `/adicionargrupo [nome]`

## 📱 Comandos

### Administrativos
- `/fechar` - Fecha o grupo
- `/abrir` - Abre o grupo  
- `/fixar [mensagem]` - Fixa uma mensagem
- `/banir @membro [motivo]` - Bane um membro
- `/bloqueartermo [palavra]` - Bloqueia uma palavra
- `/bloquearlink [dominio]` - Bloqueia um domínio
- `/removertermo [palavra]` - Remove palavra da blacklist
- `/removerlink [dominio]` - Remove domínio da blacklist
- `/listatermos` - Lista termos bloqueados
- `/adicionargrupo [nome]` - Adiciona grupo à lista permitida
- `/removergrupo [nome]` - Remove grupo da lista permitida
- `/listargrupos` - Lista grupos permitidos

### Informações
- `/status` - Status e estatísticas do grupo
- `/regras` - Exibe regras do grupo
- `/comandos` - Lista todos os comandos

### Bot
- `bot oi` - Saudação
- `bot ajuda` - Ajuda rápida
- `bot status` - Status do bot
- `bot info` - Informações do bot

## 🔒 Segurança

- Sistema anti-spam automático
- Detecção de links maliciosos
- Sistema de strikes progressivo
- Notificações para administradores
- Blacklist personalizável

## 📁 Estrutura do Projeto

```
├── functions/           # Módulos funcionais
│   ├── antiSpam.js     # Sistema anti-spam
│   ├── adminCommands.js # Comandos administrativos
│   ├── groupResponder.js # Respostas do grupo
│   ├── scheduler.js    # Agendamento automático
│   └── ...
├── index.js            # Arquivo principal
├── package.json        # Dependências
└── .env.example        # Template de configuração
```

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença ISC.

## 🆘 Suporte

Para suporte, abra uma issue no GitHub ou entre em contato com a equipe de desenvolvimento.