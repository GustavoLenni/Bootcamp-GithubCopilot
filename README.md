# Biblioteca Digital - Projeto Bootcamp Microsoft & GitHub Copilot

## Descrição

Este projeto foi desenvolvido durante o Bootcamp da Microsoft sobre GitHub Copilot. Trata-se de uma aplicação modular para gerenciamento de uma biblioteca digital, permitindo operações como empréstimo de livros, renovação de cadastro de usuários (patrons), controle de inventário e busca de exemplares.

O objetivo principal é demonstrar práticas de Clean Architecture, uso de testes automatizados, injeção de dependência e integração com arquivos JSON para persistência de dados, além de explorar o potencial do GitHub Copilot no auxílio ao desenvolvimento.

## Estrutura do Projeto

- **AZ2007LabAppM3.sln**: Arquivo de solução do Visual Studio.
- **src/**
  - **Library.ApplicationCore/**: Entidades de domínio, enums, interfaces e serviços de negócio.
  - **Library.Console/**: Aplicação de linha de comando para interação com o usuário.
  - **Library.Infrastructure/**: Implementações de acesso a dados usando arquivos JSON.
- **tests/**
  - **UnitTests/**: Testes unitários para os serviços principais.

## Funcionalidades

- Cadastro e busca de usuários (patrons)
- Empréstimo, devolução e renovação de livros
- Consulta de disponibilidade de exemplares
- Persistência de dados em arquivos JSON
- Testes unitários com xUnit e NSubstitute

## Como Executar

1. **Clone o repositório:**
   ```sh
   git clone <url-do-repositorio>
   ```

2. **Abra a solução no Visual Studio ou VS Code.**

3. **Restaure as dependências e compile:**
   ```sh
   dotnet build
   ```

4. **Execute a aplicação de console:**
   ```sh
   dotnet run --project src/Library.Console/Library.Console.csproj
   ```

5. **Execute os testes unitários:**
   ```sh
   dotnet test tests/UnitTests/UnitTests.csproj
   ```

## Tecnologias Utilizadas

- .NET 9.0
- C#
- xUnit (testes)
- NSubstitute (mocks)
- Microsoft.Extensions.DependencyInjection
- Microsoft.Extensions.Configuration

## Observações

- Os dados da biblioteca são armazenados em arquivos JSON na pasta `src/Library.Console/Json/`.
- O projeto foi desenvolvido com apoio do GitHub Copilot para acelerar a escrita de código e sugerir boas práticas.

## Licença

MIT

---

Projeto desenvolvido no Bootcamp Microsoft | GitHub Copilot
