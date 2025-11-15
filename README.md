# PROJETO-FINAL-LAB-2025-V5.5
# 🎮 Champions Boost - Plataforma de Intermediação para Serviços de Boost

Sistema Django profissional para intermediação de serviços de boost em jogos FPS competitivos, com foco em Rainbow Six Siege.

## ✅ Status: 100% Funcional

## 🎨 Design

- **Tema:** Preto, Laranja e Dourado
- **Estilo:** Moderno e inspirado no R6 Siege
- **Responsivo:** Funciona em desktop e mobile

## 🚀 Como Executar

### **Início Rápido (3 passos):**

1. **Abrir terminal** na pasta do projeto
2. **Executar:** `python manage.py runserver`
3. **Acessar:** http://127.0.0.1:8000/

### **📁 Documentação Organizada:**

Todos os guias estão na pasta `docs/` em ordem de leitura:

1. 📘 **docs/1_LEIA-ME_PRIMEIRO.txt** - Índice geral
2. 🚀 **docs/2_INICIO_RAPIDO.txt** - Guia de 3 passos
3. 📗 **docs/3_COMO_INICIAR.md** - Guia completo
4. 📙 **docs/4_GUIA_DE_USO.md** - Tutorial de uso
5. 🔐 **docs/5_ACESSO_RAPIDO.txt** - Credenciais
6. 📊 **docs/6_STATUS_SISTEMA.txt** - Status atual

### **🛠️ Scripts Úteis:**

Todos os scripts estão na pasta `scripts/`:
- `zerar_dados.py` - Limpar dados
- `verificar_usuarios.py` - Ver usuários
- `corrigir_admin.py` - Corrigir admin
- `teste_completo.py` - Testar sistema

### **URLs Importantes:**
- **Sistema:** http://127.0.0.1:8000/
- **Painel Admin:** http://127.0.0.1:8000/admin/

## 👤 Credenciais de Acesso

### 1. Admin (Administrador)
- **Gamertag:** `admin`
- **Senha:** `admin123`
- **Acesso:** Painel administrativo completo

### 2. Cliente (Solicita Boosts)
- **Gamertag:** `ProGamer123`
- **Senha:** `senha123`
- **Função:** Criar e gerenciar solicitações de boost

### 3. Booster (Realiza Boosts)
- **Gamertag:** `EliteBooster`
- **Senha:** `senha123`
- **Função:** Ver e realizar boosts para clientes

## 📋 Funcionalidades Implementadas

### RF01 - Gerenciar Cadastro de Usuário
✅ Cadastro de usuários (Cliente/Booster/Admin) com Gamertag única
✅ Login usando Gamertag e senha
✅ Edição de perfil

### RF02 - Gerenciar Autenticação
✅ Validação de credenciais
✅ Sistema de login seguro

### RF03 - Gerenciar Cadastro de Boosters
✅ Perfil específico para boosters
✅ Rank, especialização e estatísticas

### RF04 - Gerenciar Solicitações de Boost
✅ Criar solicitação com rank atual e desejado
✅ Consultar andamento com status visual
✅ Atualizar status (Booster aceita/conclui)
✅ Editar solicitação (antes do pagamento)

### RF05 - Gerenciar Pagamentos
✅ Escolher forma de pagamento (PIX, Cartão, Boleto)
✅ Validação de transação (simulada)
✅ Cálculo automático de taxa (10% plataforma)
✅ Valor do booster calculado automaticamente

### RF06 - Gerenciar Avaliações e Feedback
✅ Cliente avalia booster após conclusão
✅ Sistema de notas (1-5 estrelas)
✅ Comentários opcionais

### RF07 - Gerenciar Suporte ao Cliente
✅ Abrir chamado de suporte
✅ Consultar chamados
✅ Sistema de status (Aberto/Em Atendimento/Resolvido/Fechado)

### Extras
✅ Dashboard interativo diferenciado por tipo de usuário
✅ Painel administrativo Django completo
✅ Visual moderno inspirado em R6 Siege
✅ Cadastro de administrador com acesso ao painel

## 🎮 Jogo

- **Rainbow Six Siege** (foco exclusivo)

## 🔧 Tipos de Boost Disponíveis

- 🏆 Subir de Rank (Elo Boost)
- 🎯 Partidas de Colocação
- 💀 Melhorar K/D
- ⬆️ Subir de Nível
- 🎖️ Completar Desafios
- ⚙️ Boost Personalizado

## 🏆 Sistema de Ranks

- 🥉 Bronze
- 🥈 Prata
- 🥇 Ouro
- 💎 Platina
- 💠 Diamante
- 👑 Campeão

## 💰 Sistema de Pagamento

- **Valor Base:** R$ 50,00 por rank de diferença
- **Taxa da Plataforma:** 10% (calculada automaticamente)
- **Valor do Booster:** 90% (calculado automaticamente)
- **Formas de Pagamento:** PIX, Cartão de Crédito, Cartão de Débito, Boleto

**Exemplo:**
- Bronze → Ouro (3 ranks) = R$ 150,00
- Taxa (10%): R$ 15,00
- Booster recebe: R$ 135,00

## 📁 Estrutura do Projeto

```
PROJETO_LAB_INO_III_2025/
├── config/              # Configurações Django
│   ├── settings.py     # Configurações do projeto
│   ├── urls.py         # URLs principais
│   └── wsgi.py         # WSGI config
├── core/                # App principal
│   ├── models.py       # 6 modelos (Perfil, BoosterPerfil, SolicitacaoBoost, etc)
│   ├── views.py        # Todas as views do sistema
│   ├── urls.py         # 13 rotas configuradas
│   ├── admin.py        # Painel admin completo
│   ├── migrations/     # Migrações do banco
│   └── templates/      # 12 templates HTML
│       └── core/
│           ├── base.html
│           ├── login.html
│           ├── cadastro.html
│           ├── home.html
│           ├── solicitacao_boost.html
│           ├── listar_boosts.html
│           ├── editar_boost.html
│           ├── pagamento.html
│           ├── avaliar_boost.html
│           ├── concluir_boost.html
│           ├── suporte.html
│           └── meus_chamados.html
├── db.sqlite3          # Banco de dados SQLite
├── manage.py           # Gerenciador Django
├── README.md           # Este arquivo
├── GUIA_DE_USO.md      # Tutorial completo
├── VALIDACAO_FINAL.md  # Relatório de validação
├── RESUMO_EXECUTIVO.txt # Resumo visual
└── ACESSO_RAPIDO.txt   # Credenciais rápidas
```

## 🛠️ Comandos Úteis

```bash
# Iniciar servidor
python manage.py runserver

# Criar migrações
python manage.py makemigrations

# Aplicar migrações
python manage.py migrate

# Verificar erros
python manage.py check

# Criar usuários de teste
python criar_usuarios_teste.py

# Criar perfil de booster
python criar_booster_perfil.py

# Teste completo do sistema
python teste_completo.py
```

## 🎯 Fluxo Completo de Uso

### Como Cliente:
1. Fazer login
2. Solicitar boost (escolher ranks)
3. Ver valor calculado automaticamente
4. Escolher forma de pagamento
5. Confirmar pagamento
6. Acompanhar status
7. Avaliar booster após conclusão

### Como Booster:
1. Fazer login
2. Ver solicitações disponíveis
3. Aceitar boost
4. Realizar o serviço
5. Marcar como concluído
6. Receber 90% do valor

### Como Admin:
1. Acessar /admin/
2. Gerenciar usuários e perfis
3. Monitorar solicitações
4. Gerenciar pagamentos
5. Responder chamados de suporte
