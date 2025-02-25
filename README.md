# Wireframe-to-Code App

This Next.js application converts wireframes into code using AI models. Users can upload a wireframe image, provide a description, and select an AI model to generate the corresponding code.

## Features

-   **Wireframe Conversion:** Converts wireframe images into React code using AI.
-   **AI Model Selection:** Allows users to select from different AI models for code generation.
-   **Credit System:** Implements a credit system to manage code generation requests.
-   **User Authentication:** Uses Firebase authentication for user login and signup.
-   **Code Editor:** Integrates a code editor for viewing and editing generated code.
-   **Responsive Design:** Provides a responsive user interface.

## Technologies Used

-   [Next.js](https://nextjs.org): React framework for building the application.
-   [TypeScript](https://www.typescriptlang.org): Programming language.
-   [Tailwind CSS](https://tailwindcss.com): CSS framework for styling.
-   [Firebase](https://firebase.google.com): Authentication and storage.
-   [Drizzle ORM](https://orm.drizzle.team/): Database ORM.
-   [Neon DB](https://neon.tech/): Serverless PostgreSQL.
-   [OpenAI](https://openai.com/): AI model integration.
-   [@codesandbox/sandpack-react](https://sandpack.codesandbox.io/): Code editor.
-   [Lucide React](https://lucide.dev/): Icons.
-   [Sonner](https://sonner.emilkowal.ski/): Toast notifications.
-   [uuid4](https://www.npmjs.com/package/uuid4): UUID generator.
-   [class-variance-authority](https://www.npmjs.com/package/class-variance-authority): Utility for conditional CSS classes.
-   [clsx](https://www.npmjs.com/package/clsx): Utility for constructing className strings conditionally.
-   [tailwind-merge](https://www.npmjs.com/package/tailwind-merge): Utility to merge Tailwind CSS classes.
-   [tailwindcss-animate](https://www.npmjs.com/package/tailwindcss-animate): Animation utilities for Tailwind CSS.

## Setup

### Prerequisites

-   Node.js (version 18 or higher)
-   npm or yarn
-   Firebase project
-   Neon DB connection string
-   OpenRouter API Key

### Installation

1.  Clone the repository:

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  Install dependencies:

    ```bash
    npm install
    # or
    yarn install
    ```

3.  Create a `.env` file based on [.env.example](http://_vscodecontentref_/0) and fill in the required environment variables:

    ```
    NEXT_PUBLIC_FIREBASE_API_KEY=
    NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=
    NEXT_PUBLIC_FIREBASE_PROJECT_ID=
    NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=
    NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
    NEXT_PUBLIC_FIREBASE_APP_ID=
    NEXT_PUBLIC_FIREBASE_MESURMENT_ID=
    NEXT_PUBLIC_NEON_DB_CONNECTION_STRING=
    ```

### Database Setup

1.  Configure the database connection in [db.tsx](http://_vscodecontentref_/1) using the Neon DB connection string.
2.  Run the Drizzle Kit to generate the database schema:

    ```bash
    npx drizzle-kit generate:pg
    ```

### Firebase Setup

1.  Initialize Firebase in [firebaseConfig.tsx](http://_vscodecontentref_/2) with your Firebase project credentials.
2.  Enable Google Authentication in your Firebase project.

### Environment Variables

Ensure the following environment variables are set:

-   [NEXT_PUBLIC_FIREBASE_API_KEY](http://_vscodecontentref_/3)
-   [NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN](http://_vscodecontentref_/4)
-   [NEXT_PUBLIC_FIREBASE_PROJECT_ID](http://_vscodecontentref_/5)
-   [NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET](http://_vscodecontentref_/6)
-   [NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID](http://_vscodecontentref_/7)
-   [NEXT_PUBLIC_FIREBASE_APP_ID](http://_vscodecontentref_/8)
-   [NEXT_PUBLIC_FIREBASE_MESURMENT_ID](http://_vscodecontentref_/9)
-   [NEXT_PUBLIC_NEON_DB_CONNECTION_STRING](http://_vscodecontentref_/10)

### Running the Application

```bash
npm run dev
# or
yarn dev