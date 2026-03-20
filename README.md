## ✨ Features

-   🎯 **Dynamic Content Management**: Seamlessly manage and deliver content using Prismic.io as a headless CMS, powered by Prismic Slice Machine for flexible content structuring.
-   ⚡ **Optimized Performance**: Built with Next.js, offering Server-Side Rendering (SSR) and Static Site Generation (SSG) for fast page loads and improved user experience.
-   📱 **Responsive & Modern UI**: A beautiful and adaptive user interface crafted with Tailwind CSS for consistent styling across various devices.
-   🔐 **Type-Safe Development**: Enhanced code quality and reduced errors with TypeScript, providing strong typing throughout the application.
-   🎨 **Component-Driven Architecture**: Structured with reusable React components for maintainability and scalability.
-   🚀 **Easy Deployment**: Optimized for deployment on platforms like Vercel, ensuring a smooth transition from development to production.

## 🖥️ Screenshots

<!-- TODO: Add actual screenshots of the application, including mobile views. -->
<!-- Example: -->
<!-- ![Screenshot of Homepage](path/to/homepage-screenshot.png) -->
<!-- ![Screenshot of Product Page](path/to/product-screenshot.png) -->

## 🛠️ Tech Stack

**Frontend:**

[![Next.js](https://img.shields.io/badge/Next.js-Black?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/)

[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://react.dev/)

[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

[![Prismic](https://img.shields.io/badge/Prismic-5163BA?style=for-the-badge&logo=prismic&logoColor=white)](https://prismic.io/)

[![PostCSS](https://img.shields.io/badge/PostCSS-DD3A0A?style=for-the-badge&logo=postcss&logoColor=white)](https://postcss.org/)

**DevOps:**

[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

## 🚀 Quick Start

Follow these steps to get your development environment set up.

### Prerequisites
Make sure you have the following installed:
-   Node.js (v18.x or higher, recommended v20.x)
-   npm (comes with Node.js)
-   Git


### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/is4r0/fizzisoda.git
    cd fizzisoda
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Environment setup**
    Create a `.env` file in the root directory by copying the example:
    ```bash
    cp .env.example .env
    ```
    Configure your environment variables with your Prismic repository details:
    ```ini
    # .env
    NEXT_PUBLIC_PRISMIC_ENVIRONMENT=YOUR_PRISMIC_REPOSITORY_ID # e.g., "my-fizzisoda-repo"
    PRISMIC_ACCESS_TOKEN=YOUR_PRISMIC_ACCESS_TOKEN # Only if your repository is private
    ```

    You can find your Prismic Repository ID in the URL when you're logged into your Prismic dashboard (e.g., `https://your-repository-id.prismic.io/dashboard`).

4.  **Start development server**
    ```bash
    npm run dev
    ```

5.  **Open your browser**
    Visit `http://localhost:3000` to see the application running.

## 📁 Project Structure

```
fizzisoda/
├── public/                 # Static assets (images, fonts, etc.)
├── src/                    # Main application source code
│   ├── app/                # Next.js App Router root layout and pages
│   ├── components/         # Reusable React UI components
│   ├── slices/             # Prismic Slice Machine components
│   ├── styles/             # Global stylesheets and Tailwind CSS setup
│   └── utils/              # Utility functions and helper scripts
├── customtypes/            # Prismic custom type definitions
├── next-env.d.ts           # Next.js specific TypeScript declarations
├── next.config.mjs         # Next.js configuration file
├── package.json            # Project dependencies and scripts
├── postcss.config.js       # PostCSS configuration for Tailwind CSS
├── prismicio-types.d.ts    # Generated TypeScript types from Prismic schemas
├── set-up-content.ts       # Script for initial Prismic content setup
├── slicemachine.config.json # Prismic Slice Machine configuration
├── tailwind.config.js      # Tailwind CSS configuration file
├── tsconfig.json           # TypeScript configuration file
├── LICENSE                 # Project license
└── README.md               # Project README file
```

## ⚙️ Configuration

### Environment Variables
The project uses environment variables for sensitive data and configuration.

| Variable                      | Description                                   | Default | Required |

|-------------------------------|-----------------------------------------------|---------|----------|

| `NEXT_PUBLIC_PRISMIC_ENVIRONMENT` | Your Prismic repository ID (publicly exposed) | `null`  | Yes      |

| `PRISMIC_ACCESS_TOKEN`        | Access token for your Prismic repository      | `null`  | No (only for private repos) |

### Configuration Files
-   **`next.config.mjs`**: Configures Next.js specific settings, such as image optimization, routing, and build behavior.
-   **`tailwind.config.js`**: Defines your Tailwind CSS theme, plugins, and content paths.
-   **`postcss.config.js`**: Configures PostCSS, typically used for processing CSS with plugins like Autoprefixer and Tailwind CSS.
-   **`slicemachine.config.json`**: Configures Prismic Slice Machine, detailing where slices and custom types are located and connected to your Prismic repository.
-   **`tsconfig.json`**: TypeScript compiler options for the project.

## 🔧 Development

### Available Scripts
In the project directory, you can run:

| Command             | Description                                          |

|---------------------|------------------------------------------------------|

| `npm run dev`       | Starts the development server at `http://localhost:3000`. |

| `npm run build`     | Builds the application for production.                 |

| `npm run start`     | Starts a production Node.js server to serve the built application. |

| `npm run lint`      | Runs ESLint to identify and report on patterns found in TypeScript/JavaScript code. |

| `npm run slicemachine` | Starts the Prismic Slice Machine local development server for building and testing content slices. |


**⭐ Star this repo if think it's cool!**

Made with ❤️ by [is4r0](https://github.com/is4r0)

</div>

