# Upload Server Web

Aplicação web moderna para upload de arquivos, desenvolvida com React e TypeScript. Este projeto oferece uma interface robusta para gerenciar envios de arquivos com suporte a compressão automática de imagens e acompanhamento de progresso em tempo real.

## 🚀 Funcionalidades

- **Upload de Arquivos**: Interface intuitiva para seleção e envio de arquivos.
- **Drag & Drop**: Suporte nativo para arrastar e soltar arquivos na área de upload.
- **Compressão Automática**: Otimização de imagens no cliente antes do envio, reduzindo consumo de banda e armazenamento.
- **Acompanhamento de Progresso**:
  - Barra de progresso individual por arquivo.
  - Indicador de progresso global da fila de uploads.
- **Controle de Uploads**:
  - Capacidade de cancelar envios em andamento.
  - Botão para tentar novamente (retry) em caso de falha.
  - Interface de widget minimizável para não obstruir a navegação.

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes tecnologias principais:

- **[React](https://react.dev/)** (v19): Biblioteca para construção da interface.
- **[TypeScript](https://www.typescriptlang.org/)**: Tipagem estática para maior segurança e produtividade.
- **[Vite](https://vitejs.dev/)**: Ferramenta de build e servidor de desenvolvimento rápido.
- **[Tailwind CSS](https://tailwindcss.com/)**: Framework de utilitários para estilização.
- **[Zustand](https://zustand-demo.pmnd.rs/)**: Gerenciamento de estado simples e escalável.
- **[Immer](https://immerjs.github.io/immer/)**: Facilita a manipulação de estados imutáveis (integrado ao Zustand).
- **[Radix UI](https://www.radix-ui.com/)**: Componentes acessíveis e sem estilo (Headless UI).
- **[Framer Motion](https://www.framer.com/motion/)**: Biblioteca para animações fluidas.
- **[Axios](https://axios-http.com/)**: Cliente HTTP para realizar os uploads.

## 📦 Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- **[Node.js](https://nodejs.org/)** (versão 18 ou superior recomendada)
- Um gerenciador de pacotes (**npm**, **pnpm** ou **yarn**)
- Uma API de backend rodando para receber os uploads (por padrão, o projeto espera um servidor em `http://localhost:3333`).

## 🔧 Instalação e Execução

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/upload-server-web.git
cd upload-server-web
```

2. **Instale as dependências:**

```bash
npm install
# ou
pnpm install
# ou
yarn install
```

3. **Execute o servidor de desenvolvimento:**

```bash
npm run dev
# ou
pnpm dev
# ou
yarn dev
```

4. **Acesse a aplicação:**

Abra seu navegador e acesse `http://localhost:5173` (ou a porta indicada no terminal).

## 📂 Estrutura do Projeto

A estrutura de pastas principal é organizada da seguinte forma:

- **`src/components`**: Componentes da interface do usuário (ex: Widget de Upload).
- **`src/http`**: Funções para comunicação com a API (ex: `upload-file-to-storage.ts`).
- **`src/store`**: Lógica de estado global (Zustand) gerenciando a fila de uploads.
- **`src/utils`**: Funções utilitárias como compressão de imagem e formatação de bytes.
- **`src/App.tsx`**: Componente raiz da aplicação.

## 🤝 Como Contribuir

Contribuições são bem-vindas! Se você quiser melhorar este projeto:

1. Faça um **Fork** do repositório.
2. Crie uma Branch para sua feature (`git checkout -b feature/MinhaFeature`).
3. Faça o Commit de suas alterações (`git commit -m 'Adiciona nova feature'`).
4. Faça o Push para a Branch (`git push origin feature/MinhaFeature`).
5. Abra um **Pull Request**.

## 📝 Licença

Este projeto está desenvolvido sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.

---
Desenvolvido durante estudos de pós-graduação da **Rocketseat**.
