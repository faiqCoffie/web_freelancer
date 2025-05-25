# Firebase Studio - NextJS Starter (Freelance Platform)

This is a NextJS starter project, adapted into a freelance platform concept.

## Getting Started Locally

1. Install dependencies:
   ```bash
   npm install
   ```
2. Run the development server:
   ```bash
   npm run dev
   ```
   Open [http://localhost:9002](http://localhost:9002) (or your configured port) to view it in the browser.

## Exporting for Static Hosting (e.g., GitHub Pages)

This project is configured for static export.

1.  **Build and Export:**
    ```bash
    npm run export
    ```
    This command will build your application and then export it as static files into an `out` directory.

2.  **Deploying the `out` Directory to GitHub Pages:**
    *   **Ensure `basePath` is set:** For a repository named `larar` hosted on `username.github.io/larar/`, the `basePath` in `next.config.ts` **must** be set to `'/larar'`.
    *   **Push `out` folder:** You can commit the `out` folder to your `main` branch and configure GitHub Pages to serve from the `/out` directory on that branch.
    *   **Alternatively (Recommended):** Use a GitHub Action to automatically build, export, and deploy the contents of the `out` folder to a `gh-pages` branch. Then, configure GitHub Pages to serve from the root of the `gh-pages` branch.

    **Access URL:** Your site will be available at `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/` (e.g., `https://faiqcoffie.github.io/larar/`). Do NOT try to navigate to paths like `/src/app/`.
