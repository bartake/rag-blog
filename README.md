# RAG Learning Roadmap Blog

A comprehensive, multi-page blog covering the **RAG Learning Roadmap** from beginner foundations to advanced production systems. Each of the 20 sections includes detailed explanations for every bullet and sub-bullet in the roadmap.

## Structure

- **index.html** — Table of contents with links to all 20 sections
- **pages/** — Individual pages for each roadmap section
- **css/styles.css** — Shared styling (dark theme)

## Running Locally

```bash
npx serve .
# or
python -m http.server 8000
```

Then open `http://localhost:3000` (or the port shown).

## Topics Covered

- 🟢 **Beginner** (1–4): AI/NLP basics, information retrieval, vector databases, RAG core
- 🟡 **Intermediate** (5–9): Data prep, embeddings, retrieval, prompts, hands-on implementation
- 🟠 **Advanced** (10–13): Advanced retrieval, evaluation, scaling, production
- 🔴 **Expert** (14–20): Security, cost, advanced patterns, enterprise use cases, observability, future trends

## Publish to GitHub

The project is a Git repo on `main` with an initial commit. To push it to **your** GitHub account:

1. **Log in** with the [GitHub CLI](https://cli.github.com/) (install if needed: `winget install GitHub.cli`):

   ```bash
   gh auth login
   ```

   Follow the prompts (HTTPS, authenticate via browser, or paste a personal access token).

2. **Create the remote repo and push** from this folder:

   ```bash
   cd rag-blog
   gh repo create rag-blog --public --source=. --remote=origin --push
   ```

   Change `rag-blog` to your preferred repository name. Use `--private` instead of `--public` if you want a private repo.

**If you already created an empty repo on GitHub**, add it and push:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

Replace `YOUR_USERNAME` and `YOUR_REPO` with your GitHub username and repository name.
