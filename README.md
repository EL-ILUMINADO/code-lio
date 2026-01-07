# Code Lio - SaaS Code Editor

[![Live Demo](https://img.shields.io/badge/demo-online-green.svg)](https://code-lio.vercel.app)
[![Author](https://img.shields.io/badge/author-EL--ILUMINADO-blue.svg)](https://github.com/EL-ILUMINADO)

**Code Lio** is a powerful, modern SaaS-based code editor built for developers who need a seamless coding experience directly in their browser. It features real-time code execution, snippet management, and community interaction, all wrapped in a sleek, responsive interface.

## 🚀 Features

- **Multi-Language Support**: Write and execute code in various programming languages directly from your browser.
- **Monaco Editor Integration**: Enjoy a VS Code-like editing experience with syntax highlighting, auto-completion, and error detection.
- **Code Execution Engine**: Powered by the Piston API to run code safely and efficiently.
- **Snippet Management**: Save your favorite code snippets, title them, and organize them for easy access.
- **Community & Social**:
  - **Star Snippets**: Like and save useful snippets from other users.
  - **Comments**: Engage with the community by discussing code snippets.
- **Pro Subscription (Lemon Squeezy)**:
  - Unlimited code executions.
  - Exclusive Pro badge.
  - Priority support.
- **Authentication**: Secure and easy sign-in via Clerk (GitHub, Google, Email).
- **Responsive Design**: Fully responsive UI built with Tailwind CSS and Framer Motion for smooth animations.

## 🛠 Tech Stack

- **Framework**: [Next.js 16](https://nextjs.org/) (App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Frontend**: [React 19](https://react.dev/), [Tailwind CSS](https://tailwindcss.com/), [Framer Motion](https://www.framer.com/motion/)
- **Backend / Database**: [Convex](https://www.convex.dev/) (Real-time database & backend functions)
- **Authentication**: [Clerk](https://clerk.com/)
- **Code Editor**: [@monaco-editor/react](https://github.com/suren-atoyan/monaco-react)
- **Payments**: [Lemon Squeezy](https://www.lemonsqueezy.com/)
- **Icons**: [Lucide React](https://lucide.dev/)

## 📂 Project Structure

```bash
├── convex/             # Backend functions & schema (Convex)
├── public/             # Static assets
├── src/
│   ├── app/            # Next.js App Router pages & layouts
│   ├── components/     # Reusable UI components
│   ├── hooks/          # Custom React hooks
│   ├── store/          # State management (Zustand)
│   ├── types/          # TypeScript type definitions
│   └── middleware.ts   # Clerk authentication middleware
├── .env.local          # Environment variables
└── package.json        # Project dependencies
```

## ⚡ Getting Started

### Prerequisites

Ensure you have the following installed:

- Node.js (v18 or later)
- npm, yarn, pnpm, or bun

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/EL-ILUMINADO/code-lio.git
    cd code-lio
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    # or
    pnpm install
    ```

3.  **Set up Environment Variables:**

    Create a `.env.local` file in the root directory and add the following keys:

    ```env
    # Convex
    CONVEX_DEPLOYMENT=
    NEXT_PUBLIC_CONVEX_URL=

    # Clerk Auth
    NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
    CLERK_SECRET_KEY=

    # Lemon Squeezy (Payments)
    LEMON_SQUEEZY_API_KEY=
    LEMON_SQUEEZY_WEBHOOK_SECRET=
    NEXT_PUBLIC_LEMON_SQUEEZY_STORE_ID=
    ```

4.  **Run the Development Server:**

    You need to run both the Next.js frontend and the Convex backend function sync:

    ```bash
    npm run dev
    ```

    _Note: Ensure `npx convex dev` is running (usually handled by the dev script or run separately)._

5.  **Open the App:**

    Visit [http://localhost:3000](http://localhost:3000) in your browser.

## 🚀 Deployment

The easiest way to deploy this application is using **Vercel**.

1.  Push your code to a GitHub repository.
2.  Import the project into Vercel.
3.  Add the environment variables (from `.env.local`) in the Vercel project settings.
4.  Deploy!

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

Built with ❤️ by [EL-ILUMINADO](https://github.com/EL-ILUMINADO)
