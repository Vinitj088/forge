# next-forge

**Production-grade Turborepo template for Next.js apps.**

# Run the Web App

Here's a step-by-step guide to get your web app running, focusing only on the web development part:

## Step 1: Install Bun

First, you need to install Bun, which is the package manager used in this project:
here's the link of the website => https://bun.sh/

```bash
powershell -c "irm bun.sh/install.ps1 | iex"
```

for linux/macos

```bash
curl -fsSL https://bun.sh/install | bash
```

After installation, restart your terminal or command prompt.

## Step 2: Clone the Repository

```bash
git clone https://github.com/Vinitj088/forge
```

Replace `your-username/your-repo-name` with your actual GitHub repository URL.

## Step 3: Install Dependencies

```bash
cd apps\web
bun install
```

## Step 4: Set Up Environment Variables

You already have your `.env.local` file set up with the Resend email configuration. Make sure any other required variables are filled in as needed.

## Step 5: Run the Development Server

```bash
bun dev
```

This will start the development server for the web app only. You should be able to access it at http://localhost:3001 (based on your NEXT_PUBLIC_WEB_URL setting).

## Troubleshooting Tips

1. If you encounter any errors about missing dependencies:
   ```bash
   bun install [package-name]
   ```

2. If you get environment variable validation errors, check your `.env.local` file to make sure all required variables are set.

3. If the server fails to start, try running with verbose logging:
   ```bash
   bun --verbose dev
   ```

4. To reset your environment if things get messy:
   ```bash
   bun clean
   bun install
   ```

That's it! You should now have the web app running locally for development.
