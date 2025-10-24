# 🚗 MidCar Engenharia - Sistema de Controle de Contatos

## 📋 Sobre o Projeto

Sistema de gestão completo para oficina mecânica desenvolvido em **ASP.NET Core 5.0** com **Entity Framework Core** e **SQL Server LocalDB**. O sistema permite o controle de clientes, veículos, ordens de serviço e orçamentos de forma integrada e eficiente.

## 🎯 Funcionalidades

### 👥 **Gestão de Usuários**
- Sistema de autenticação e autorização
- Controle de perfis (Admin, Usuário)
- Login seguro com criptografia de senhas

### 👤 **Gestão de Clientes**
- Cadastro completo de clientes
- Informações pessoais e de contato
- Histórico de veículos e serviços
- Busca e filtros avançados

### 🚗 **Gestão de Veículos**
- Cadastro de veículos por cliente
- Informações técnicas completas (placa, modelo, marca, ano, etc.)
- Controle de quilometragem e observações
- Histórico de serviços realizados

### 🔧 **Ordens de Serviço**
- Criação e acompanhamento de OS
- Numeração automática sequencial
- Controle de status (Aberta, Em Andamento, Finalizada, Cancelada)
- Gestão de datas (abertura, início, finalização)
- Mecânico responsável (Milton Diego como padrão)
- Cálculo de valores e observações

### 💰 **Orçamentos**
- Criação de orçamentos detalhados
- Numeração automática sequencial
- Controle de status (Pendente, Aprovado, Rejeitado, Convertido em OS)
- Gestão de validade e aprovação
- Conversão automática em Ordem de Serviço
- Cálculo de valores totais

## 🛠️ Tecnologias Utilizadas

- **Backend:** ASP.NET Core 5.0
- **ORM:** Entity Framework Core
- **Banco de Dados:** SQL Server LocalDB
- **Frontend:** Razor Pages com Bootstrap
- **Autenticação:** ASP.NET Core Identity
- **Validação:** Data Annotations
- **Padrão:** Repository Pattern

## 📁 Estrutura do Projeto

```
ControleDeContatos/
├── Controllers/ # Controladores MVC
├── Models/ # Modelos de dados
├── Repositorio/ # Repositórios (Repository Pattern)
├── Views/ # Views Razor
├── wwwroot/ # Arquivos estáticos (CSS, JS, Imagens)
├── Data/ # Contexto do Entity Framework
└── Migrations/ # Migrações do banco de dados
```

## 🚀 Como Executar

### Pré-requisitos
- .NET 5.0 SDK ou superior
- SQL Server LocalDB
- Visual Studio 2019/2022 ou VS Code

### Instalação

1. **Clone o repositório:**
```bash
git clone https://github.com/Claudioofc/MIDCARENGENHARIA.git
cd MIDCARENGENHARIA
```

2. **Restaure as dependências:**
```bash
dotnet restore
```

3. **Execute as migrações:**
```bash
dotnet ef database update
```

4. **Execute a aplicação:**
```bash
dotnet run
```

5. **Acesse a aplicação:**
- URL: `http://localhost:5000`
- Login: `admin`
- Senha: `123456`

## 🗄️ Banco de Dados

### Tabelas Principais

- **Usuarios:** Controle de usuários e autenticação
- **Clientes:** Dados dos clientes da oficina
- **Veiculos:** Veículos dos clientes
- **OrdensServico:** Ordens de serviço
- **Orcamentos:** Orçamentos e propostas
- **ItensOrcamento:** Itens detalhados dos orçamentos

### Connection String
```json
{
 "ConnectionStrings": {
 "DataBase": "Server=(localdb)\\mssqllocaldb;Database=DB_SistemaContatos;Trusted_Connection=true;MultipleActiveResultSets=true"
 }
}
```

## 👨‍💻 Usuário Padrão

- **Login:** admin
- **Senha:** 123456
- **Perfil:** Administrador

## 🔧 Configurações

### Mecânico Padrão
- **Nome:** Milton Diego
- Configurado automaticamente em novas Ordens de Serviço

### Numeração Automática
- **Ordens de Serviço:** OS0001, OS0002, OS0003...
- **Orçamentos:** ORC0001, ORC0002, ORC0003...

## 📊 Funcionalidades por Módulo

### Dashboard
- Visão geral do sistema
- Estatísticas de clientes, veículos e serviços
- Gráficos e relatórios básicos

### Clientes
- ✅ Cadastro completo
- ✅ Edição e exclusão
- ✅ Busca por nome, email, telefone
- ✅ Histórico de veículos

### Veículos
- ✅ Cadastro por cliente
- ✅ Informações técnicas completas
- ✅ Controle de ativo/inativo
- ✅ Histórico de serviços

### Ordens de Serviço
- ✅ Criação automática
- ✅ Controle de status
- ✅ Gestão de datas
- ✅ Mecânico responsável
- ✅ Cálculo de valores

### Orçamentos
- ✅ Criação detalhada
- ✅ Aprovação/Rejeição
- ✅ Controle de validade
- ✅ Conversão em OS
- ✅ Cálculo automático

## 🔒 Segurança

- Autenticação obrigatória
- Controle de sessão
- Criptografia de senhas
- Validação de dados
- Proteção contra SQL Injection

## 📈 Melhorias Futuras

- [ ] Relatórios avançados
- [ ] Integração com WhatsApp
- [ ] Sistema de notificações
- [ ] Backup automático
- [ ] API REST
- [ ] Aplicativo mobile

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Desenvolvedor

**Claudio Oliveira**
- GitHub: [@Claudioofc](https://github.com/Claudioofc)

## 📞 Suporte

Para suporte e dúvidas, entre em contato através do GitHub Issues.

---

**Desenvolvido com ❤️ para MidCar Engenharia**
