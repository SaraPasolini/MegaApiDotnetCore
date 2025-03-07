# 📄 Resumo da API Mega Man Robots

## 📌 Visão Geral
A **Mega Man Robots API** é um serviço backend desenvolvido com **.NET Core 3.1**, projetado para fornecer dados em formato **JSON** sobre os chefes da franquia **Mega Man**. 

Utilizando **Entity Framework Core** e outros recursos modernos do ecossistema .NET, esta API permite o acesso eficiente e estruturado às informações dos robôs, garantindo um serviço robusto e escalável.

---

## 🚀 Funcionalidades Principais
- 📋 **Fornecimento de dados sobre os chefes da série Mega Man**
- 📡 **Pontos de extremidade (endpoints) bem estruturados** para recuperar, adicionar e gerenciar dados
- 🔧 **Uso do Entity Framework Core** para a manipulação e persistência de dados
- 🏗 **Arquitetura baseada em princípios RESTful** para facilitar a integração

---

## 🔗 Endpoints Disponíveis

| Método  | Endpoint                 | Descrição                                          |
|---------|--------------------------|--------------------------------------------------|
| **GET**  | `/api/v1/robos`         | Retorna uma lista de todos os robôs             |
| **GET**  | `/api/v1/robos/{id}`    | Retorna detalhes de um robô específico pelo ID  |
| **POST** | `/api/v1/robos`         | Cria uma nova entrada de robô                    |

---

## 🔧 Tecnologias e Dependências

- **Entity Framework Core** – ORM para gerenciamento de dados
- **Design de API RESTful** – Comunicação eficiente entre cliente e servidor
- **Injeção de Dependência** – Flexibilidade e melhor capacidade de teste
- **Newtonsoft.Json** – Serialização e desserialização de JSON

### 📦 Dependências Principais

| Pacote | Versão | Link |
|--------|--------|------|
| Microsoft.EntityFrameworkCore | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/) |
| Microsoft.EntityFrameworkCore.Design | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design/) |
| Microsoft.EntityFrameworkCore.SqlServer | 3.1.8 | [NuGet](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer/) |
| Newtonsoft.Json | 12.0.2 | [NuGet](https://www.nuget.org/packages/Newtonsoft.Json/) |

---

## 📂 Estrutura do Projeto

```
📦 src
 ├── 📂 Controllers      # Rotas para os endpoints
 ├── 📂 Models           # Modelos de dados
 ├── 📂 Services         # Regras de negócio
 ├── 📂 Middlewares      # Funções intermediárias entre requisição e resposta
 ├── 📂 Database         # Estruturas relacionadas ao banco de dados
 │   ├── 📂 DTOs             # Modelos de entrada e saída (Data Transfer Objects)
 │   ├── 📂 EntityFramework  # Arquivos relacionados ao ORM
 │   │     ├── 📂 Context         # Configuração do contexto do Entity Framework
 │   │     ├── 📂 Migrations      # Arquivos de migração do banco de dados
 │   ├── 📂 Repositories     # Implementação do padrão Repository
```

---

## 📜 Licença
Este software é licenciado sob os termos do [MIT](LICENSE).
