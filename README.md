# edilsonfj.com

O *edilsonfj.com* é um site de portfólio pessoal e profissional de desenvolvimento full-stack, com foco na apresentação de experiências e serviços de desenvolvimento de softwares, aplicações, sites e interfaces web. A plataforma oferece uma interface institucional e uma aplicação para prestação de serviços freelancer, com gerenciamento de clientes e serviços.

## Requisitos

### Requisitos Funcionais

#### Interface Inicial

- **Home:** Breve apresentação do desenvolvedor, serviços oferecidos e testemunhos/indicações.
- **Sobre Mim:** Informações sobre a experiência e habilidades do desenvolvedor.
- **Serviços/Produtos:** Detalhes sobre os serviços e produtos oferecidos, incluindo desenvolvimento de software, aplicações web e mobile, e criação de sites.
- **Portfólio:** Exibição de projetos anteriores com descrições e imagens.
- **Contato:** Formulário de contato para clientes potenciais.
- **Blog:** Publicações sobre tecnologia, projetos e experiências pessoais.
- **Área de Cliente:** Botão para acessar a área de cliente.

#### Área do Cliente

- **Cadastro:** Criar, visualizar e editar dados do cliente.
- **Serviços:** Adquirir serviços formatados ou solicitar um serviço personalizado.
- **Contratos:** Visualizar, assinar, acompanhar e imprimir contratos.
- **Projetos:** Acompanhar o andamento dos projetos contratados.
- **Financeiro:** Gerenciar pagamentos e visualizar faturas.

#### Área de Gestão

- **Clientes:** Visualizar e gerenciar informações dos clientes.
- **Serviços:** Criar, visualizar, editar e excluir serviços.
- **Contratos:** Criar, visualizar, assinar e editar contratos.
- **Projetos:** Gerenciar o andamento dos projetos.
- **Financeiro:** Gerenciar informações financeiras, incluindo orçamentos, pagamentos e relatórios.

### Regras de Negócio

- **Controle de Acesso:** Diferenciação de permissões entre clientes e administradores.
- **Cálculo de Margens:** Regras para cálculo automático de margens de preço dos serviços.
- **Validação de Dados:** Validação dos dados do cliente e do projeto para garantir integridade e consistência.
- **Exportação de Orçamento:** Geração de orçamento em PDF com todas as informações detalhadas.

### Requisitos Não-Funcionais

- **Segurança:**
  - Autenticação e autorização seguras (ex: OAuth2, JWT).
  - Proteção contra ataques comuns como SQL Injection, XSS, CSRF.
  - Criptografia de dados sensíveis (ex: informações de clientes, detalhes de orçamentos).
- **Desempenho:**
  - Respostas rápidas da API com tempos de resposta baixos.
  - Suporte para grande volume de acessos e dados.
- **Escalabilidade:**
  - Arquitetura preparada para crescimento do número de orçamentos e usuários.
  - Uso de serviços em nuvem para balanceamento de carga e armazenamento.
- **Usabilidade:**
  - Interface de usuário intuitiva e fácil de navegar.
  - Design responsivo para dispositivos móveis e diferentes tamanhos de tela.
- **Manutenibilidade:**
  - Código bem documentado e modularizado.
  - Testes unitários e de integração para garantir a qualidade do código.
- **Conformidade:**
  - Adesão a regulamentações de proteção de dados (ex: GDPR, LGPD).
  - Conformidade com padrões de acessibilidade web (ex: WCAG).

## 🛠️ Construído com

* [Typescript](https://www.typescriptlang.org/docs/) - Linguagem de Programação
* [NestJS](https://docs.nestjs.com/) - Framework de Desenvolvimento Backend
* [Postgres](https://www.postgresql.org/docs/) - Banco de Dados Relacional
* [Next.js](https://nextjs.org/docs) - Framework de Desenvolvimento Frontend
* [Tailwind](https://tailwindcss.com/docs/) - Biblioteca de Estilização
* [Lucide](https://lucide.dev/docs) - Biblioteca de Componentes e Ícones

## Estrutura de Pastas e Tecnologias

### Backend

- **Framework:** NestJS
- **Gerenciamento de Pacotes:** npm
- **Autenticação e Autorização:** JWT com Passport
- **Conexão com o Banco de Dados:** ORM Prisma
- **Variáveis de Ambiente:** Dotenv

#### Ferramentas e Bibliotecas
- **Sistema de Testes:** Jest
- **Linting e Formatação:** ESLint, Prettier
- **Documentação:** Swagger com NestJS
- **Validação de Dados:** Class-validator e Class-transformer

#### Estrutura de Pastas
- `src/`
  - `controllers/`
  - `models/`
  - `modules/`
  - `services/`
  - `utils/`
  - `middlewares/`
  - `config/`

### Frontend

#### Essenciais
- **Framework:** Next.js
- **Estilização:** Tailwind CSS
- **Componentes e Ícones:** Lucide
- **Gerenciamento de Estado:** Redux
- **Roteamento:** Next.js Routing

#### Ferramentas e Bibliotecas
- **Sistema de Testes:** Jest
- **Linting e Formatação:** ESLint, Prettier
- **SEO e Acessibilidade:** Implementação com Next.js para otimização de SEO

#### Estrutura de Pastas
- `src/`
  - `components/`
  - `pages/`
  - `hooks/`
  - `context/`
  - `utils/`
  - `assets/`
  - `styles/`

### Database

#### Essenciais
- **ORM:** Prisma
- **Migrations:** Prisma Migrate
- **Seed Data:** Scripts para popular o banco de dados

#### Ferramentas e Bibliotecas
- **ORM:** Prisma
- **Migrations:** Prisma Migrate
- **Seed Data:** Scripts personalizados
- **Gerenciamento de Banco de Dados:** pgAdmin (para PostgreSQL), MongoDB Compass (para MongoDB)

#### Estrutura de Pastas
- `prisma/`
  - `schema.prisma`
  - `migrations/`
  - `seed.ts`