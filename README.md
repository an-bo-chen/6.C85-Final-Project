# 6.C85 Final Project: Team AYJE UrbanVis Studio

## Getting Started

To get started with this project, first clone the repository and install the dependencies:

```bash
# Clone the repository
git clone git@github.com:an-bo-chen/6.C85-Final-Project.git

# Navigate into the project directory
cd 6.C85-Final-Project

# Install dependencies
npm install
```

For the best development experience, install these VSCode extensions:
- Svelte for VS Code
- ESLint
- Prettier - Code formatter

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Testing

### Using Storybook

Storybook is used to develop and test UI components in isolation. To start Storybook, run:

```bash
npm run storybook
```

This will launch the Storybook development server, where you can interact with and test individual components. You can also build a static version of Storybook for deployment:

```bash
npm run build-storybook
```

### Using Playwright

Playwright is used for end-to-end testing. To run Playwright tests, use:

```bash
npm run test:e2e
```

This will execute all end-to-end tests defined in the `e2e` directory. You can also run Playwright in headed mode for debugging:

```bash
npx playwright test --headed
```

To generate a new Playwright test, use the following command to record interactions:

```bash
npx playwright codegen
```

This will open a browser where you can record actions, which will be saved as a test script.

## Available Commands

```bash
# Install dependencies
npm install

# Development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run tests
npm run test

# Run unit tests
npm run test:unit

# Run end-to-end tests
npm run test:e2e

# Run linting
npm run lint

# Format code with Prettier
npm run format

# Start Storybook
npm run storybook

# Build Storybook static site
npm run build-storybook
```

## Project Structure

```
6.C85-Final-Project/
├── .storybook/               # Configuration files for Storybook, a UI component explorer
├── e2e                       # End-to-end test files and configurations
├── src/                      # Main source code for the application
│   ├── lib/                  # Reusable library code, including components and utilities
│   │   └── ...               # Individual components, helper functions, etc.
│   ├── routes/               # SvelteKit route definitions and associated logic
│   │   └── ...               # Layout and pages
│   └── stories/              # Storybook stories for UI components
│   │   └── ...               # UI components to test out
├── static/                   # Static assets like images, fonts, and other files served as-is
└── visualization-scripts/    # Scripts and tools for data visualization
```