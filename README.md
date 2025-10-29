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

## Publish to GitHub (SSH)

This repo is on branch `main` with commits. Pushing uses **SSH** (`git@github.com:...`), not HTTPS.

1. **Create an empty repository** on GitHub ([new repository](https://github.com/new)): choose a name (e.g. `rag-blog`), **do not** add a README, `.gitignore`, or license (avoids merge conflicts).

2. **Point `origin` at that repo** (skip if it already matches):

   ```bash
   git remote add origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
   ```

   To change an existing remote:

   ```bash
   git remote set-url origin git@github.com:YOUR_USERNAME/YOUR_REPO.git
   ```

3. **Push**:

   ```bash
   git push -u origin main
   ```

If you see `ERROR: Repository not found`, the GitHub repo does not exist yet or the URL does not match your account/org.

**Optional — [GitHub CLI](https://cli.github.com/)** (after `gh auth login`):  
`gh repo create rag-blog --public --source=. --remote=origin --push` (creates the repo and pushes; can use SSH for Git operations if configured in `gh`).
