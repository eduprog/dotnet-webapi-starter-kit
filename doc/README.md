# Documentação Técnica - FullStackHero .NET 10 Starter Kit

Esta documentação foi criada para fornecer um guia completo e técnico sobre o funcionamento do **FullStackHero .NET 10 Starter Kit**.

## 📚 Estrutura da Documentação

A documentação está organizada em 6 seções principais, cada uma em um arquivo HTML separado:

### 1. [index.html](index.html) - Página Inicial

- Visão geral do projeto
- Links para todas as seções
- Recursos principais destacados
- Quick start guide

### 2. [visao-geral.html](visao-geral.html) - Visão Geral

- O que é o FullStackHero
- Arquitetura Vertical Slice
- Stack tecnológica completa
- Princípios de design (DDD, CQRS, Clean Architecture)
- Estrutura de diretórios detalhada

### 3. [building-blocks.html](building-blocks.html) - Building Blocks

Documentação detalhada de todos os componentes reutilizáveis:

- **Core**: Entidades de domínio, domain events, exceptions
- **Persistence**: EF Core, Repository Pattern, Specifications
- **Caching**: Redis distributed cache, hybrid cache
- **Jobs**: Hangfire para background jobs
- **Mailing**: Envio de emails com MailKit
- **Storage**: Abstração para armazenamento de arquivos
- **Web**: Auth, CORS, OpenAPI, Rate Limiting, OpenTelemetry
- **Eventing**: Event bus para integração entre módulos

### 4. [modulos.html](modulos.html) - Módulos

Explicação completa dos módulos de negócio:

- **Identity Module**: ASP.NET Identity + JWT, gestão de usuários, roles e permissions
- **Multitenancy Module**: Finbuckle MultiTenant, isolamento de dados por tenant
- **Auditing Module**: Auditoria de segurança, exceções e atividades
- Como criar seus próprios módulos

### 5. [padroes-codigo.html](padroes-codigo.html) - Padrões de Código

Guia de padrões e práticas:

- **CQRS Pattern**: Commands vs Queries
- **Mediator Pattern**: Desacoplamento e organização
- **Minimal APIs**: Estrutura de endpoints
- **Repository & Specification**: Acesso a dados testável
- **Domain Events**: Comunicação dentro do domínio
- Estrutura completa de uma feature

### 6. [configuracao.html](configuracao.html) - Configuração

Todas as configurações do sistema:

- **DatabaseOptions**: PostgreSQL e SQL Server
- **CachingOptions**: Redis
- **JwtOptions**: Autenticação JWT
- **CorsOptions**: Cross-Origin Resource Sharing
- **OpenTelemetry**: Observabilidade
- Outras configurações (Mailing, Hangfire, Storage)
- Exemplo completo de appsettings.json

### 7. [execucao.html](execucao.html) - Execução

Como executar e fazer deploy:

- Pré-requisitos
- Executar com .NET Aspire (recomendado)
- Executar API standalone
- Executar testes (unit, integration, architecture)
- Build & Publish
- Docker e containerização
- Deploy com Terraform na AWS
- Troubleshooting
- Comandos úteis

```bash
# Executando da pasta raiz do projeto
dotnet run --project .\src\Playground\FSH.Playground.AppHost\FSH.Playground.AppHost.csproj
```

## 🎨 Tecnologias Usadas na Documentação

- **HTML5**: Estrutura semântica
- **Tailwind CSS**: Framework CSS via CDN para estilização moderna e responsiva
- **Font Awesome**: Ícones consistentes em toda a documentação
- **Design Responsivo**: Compatível com desktop, tablet e mobile

## 🚀 Como Visualizar

### Opção 1: Abrir Diretamente no Navegador

1. Navegue até a pasta `doc/`
2. Clique duas vezes em `index.html`
3. O arquivo abrirá no seu navegador padrão

### Opção 2: Servidor Local (Recomendado)

Para melhor experiência, sirva os arquivos através de um servidor HTTP local:

**Python:**

```bash
cd doc
python -m http.server 8000
# Acesse: http://localhost:8000
```

**Node.js (http-server):**

```bash
cd doc
npx http-server -p 8000
# Acesse: http://localhost:8000
```

**.NET:**

```bash
cd doc
dotnet tool install --global dotnet-serve
dotnet serve -p 8000
# Acesse: http://localhost:8000
```

## 📱 Navegação

Cada página possui:

- **Barra de navegação superior**: Link para voltar ao índice
- **Navegação inferior**: Links para página anterior e próxima
- **Seções ancoradas**: Links internos para navegação rápida
- **Design responsivo**: Adaptação automática para diferentes tamanhos de tela

## 🎯 Características

- ✅ **Totalmente em Português (pt-BR)**
- ✅ **Exemplos de código com syntax highlighting**
- ✅ **Diagramas em ASCII art**
- ✅ **Cards interativos com hover effects**
- ✅ **Gradientes e cores consistentes**
- ✅ **Sem dependências externas** (exceto CDNs de Tailwind e Font Awesome)
- ✅ **Pronto para impressão/PDF** (se necessário)

## 📖 Conteúdo Coberto

A documentação cobre:

- ✅ Arquitetura e design patterns
- ✅ Todos os building blocks em detalhe
- ✅ Todos os módulos (Identity, Multitenancy, Auditing)
- ✅ Padrões de código (CQRS, Mediator, Specifications)
- ✅ Configuração completa (appsettings, env vars)
- ✅ Execução (Aspire, standalone, Docker, Terraform)
- ✅ Testes (unit, integration, architecture)
- ✅ Troubleshooting e comandos úteis

## 🔄 Atualizações

Para atualizar a documentação:

1. Edite os arquivos HTML correspondentes
2. Mantenha a consistência de cores e estilos
3. Use as mesmas classes Tailwind para manter a uniformidade
4. Teste em múltiplos navegadores

## 📝 Notas

- Todos os exemplos de código são baseados no código real do projeto
- As cores seguem o tema do projeto (azul primário, roxo secundário, verde accent)
- Font Awesome é usado para ícones consistentes
- Tailwind CSS via CDN (sem necessidade de build)

## 🙏 Créditos

Documentação criada para o projeto **FullStackHero .NET 10 Starter Kit** por Mukesh Murugan.

---

**Última atualização:** Janeiro de 2026  
**Versão do projeto:** 10.0.0-rc.1
