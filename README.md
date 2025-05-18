# Next.js RTK Starter

A modern and scalable starter template for **Next.js**, following best practices with clean architecture based on **Feature-Sliced Design (FSD)**. This setup is ready to go with **TypeScript**, **Redux Toolkit (RTK)**, **RTK Query**, **ESLint**, **Prettier**, **Commitlint**, and **Husky**.

## 🚀 Features

- **Next.js** – The production-ready React framework.
- **TypeScript** – Static typing for JavaScript.
- **Redux Toolkit (RTK)** – Efficient and scalable state management.
- **RTK Query** – Built-in data fetching and caching.
- **Feature-Sliced Design (FSD)** – Modular architecture for large applications.
- **Prettier** – Code formatter for consistent style.
- **ESLint** – Code linter to ensure code quality.
- **Commitlint** – Enforce conventional commit messages.
- **Husky** – Git hooks for pre-commit and commit-msg checks.

## 📦 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Hossein-i/nextjs-rtk-starter.git
   ```

2. Navigate to the project directory:

   ```bash
   cd nextjs-rtk-starter
   ```

3. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

### Running the Development Server

Start the dev server:

```bash
npm run dev
# or
yarn dev
```

Then open [http://localhost:3000](http://localhost:3000) in your browser.

## 🧱 Project Structure (FSD)

This project uses the **Feature-Sliced Design** architecture to enhance scalability and maintainability:

```bash
src/
├── app/           # Next.js app router (layouts, pages)
├── entities/      # Business entities like user, product
│   ├── api/       # Entity-related API logic
│   ├── model/     # Types, stores, services
│   └── ui/        # Entity-specific UI components
├── features/      # Independent, reusable features
│   ├── api/       # Feature-specific API calls
│   ├── config/    # Feature-level configuration
│   ├── lib/       # Internal libraries for the feature
│   ├── model/     # Logic, stores, types
│   └── ui/        # UI for feature interactions
├── shared/        # Cross-cutting code (global utils, UI, config)
│   ├── api/       # API client setup and base query
│   ├── config/    # App-wide config and env vars
│   ├── i18n/      # Internationalization setup
│   ├── lib/       # Utilities and helper functions
│   ├── styles/    # Global styles and themes
│   └── ui/        # Design system components
├── views/         # Top-level views composed of widgets/features
└── widgets/       # UI blocks that encapsulate full use cases
```

## ⚙️ State Management & Data Fetching

This template comes with:

- **Redux Toolkit** for managing global app state.
- **RTK Query** for fetching, caching, and managing server state with minimal boilerplate.

> Store setup and slices can be found in `shared/api` and `features/model`.

## 🧹 Code Quality Tools

### Prettier

Ensures consistent code formatting:

```bash
npm run format
# or
yarn format
```

### ESLint

Checks code for style and quality issues:

```bash
npm run lint
# or
yarn lint
```

### Commitlint

Enforces [Conventional Commits](https://www.conventionalcommits.org/) for all commit messages:

```bash
npm run commit
# or
yarn commit
```

## 🔒 Git Hooks (Husky)

Husky ensures quality checks before code is committed:

- **Pre-commit**: Runs ESLint and Prettier
- **Commit-msg**: Validates commit message format

## 🤝 Contributing

We welcome contributions! To get started:

1. Fork the repo.
2. Create a new branch: `git checkout -b feature/YourFeatureName`.
3. Commit your changes: `git commit -m 'feat: Add awesome feature'`.
4. Push the branch: `git push origin feature/YourFeatureName`.
5. Open a Pull Request.

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

## 🙌 Acknowledgments

- [Next.js Docs](https://nextjs.org/docs)
- [Feature-Sliced Design](https://feature-sliced.design/)
- [Redux Toolkit](https://redux-toolkit.js.org/)
- [RTK Query](https://redux-toolkit.js.org/rtk-query/overview)
- [Conventional Commits](https://www.conventionalcommits.org/)
