# Contributing

Thanks for stopping by! Contributions are welcome across all my repos — whether that's fixing a bug, improving docs, adding a feature, or just pointing out that something is broken.

These guidelines apply to any repo in this account that doesn't have its own `CONTRIBUTING.md`.

---

## Before you start

- **Check open issues first.** Someone may already be working on the same thing.
- **Open an issue before large changes.** For significant refactors or new features, a quick issue to discuss the approach saves everyone time.
- **Small PRs are easier to review.** Prefer focused, single-purpose changes over large sprawling ones.

---

## How to contribute

### 1. Fork and clone

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### 2. Create a branch

Use a descriptive name:

```bash
git checkout -b fix/broken-terraform-output
git checkout -b feat/add-docker-compose-override
git checkout -b docs/improve-setup-instructions
```

### 3. Make your changes

- Follow the existing code style — consistency matters more than perfection
- Keep changes focused on one thing
- Update the README or relevant docs if your change affects behaviour or usage
- Test locally before pushing (see the repo's README for how to run things)

### 4. Commit clearly

```bash
git commit -m "fix: correct variable reference in main.tf"
git commit -m "feat: add support for custom domain in nginx config"
git commit -m "docs: clarify pre-requisites in README"
```

Conventional Commits format is preferred but not required — just be descriptive.

### 5. Open a pull request

Fill out the PR template. The more context you provide, the faster it gets reviewed.

---

## Types of contributions

| Type | Notes |
|---|---|
| 🐛 Bug fixes | Always welcome — please include steps to reproduce |
| 📝 Docs improvements | Typos, clarifications, better examples — great first contributions |
| ✨ New features | Open an issue first for anything non-trivial |
| 🔧 Refactors | Fine as long as behaviour doesn't change unexpectedly |
| 🧪 Tests / validation | Highly appreciated — most repos could use more |

---

## What to expect

- I review PRs when I can, but response times vary — I'm not running a product, just sharing work
- If a PR sits for a while, feel free to ping in the issue thread
- Not every PR will be merged — sometimes the direction just doesn't fit, but I'll always explain why

---

## Code style

There's no strict style guide across all repos, but the general idea:

- **Shell scripts**: POSIX-compatible where possible, `shellcheck`-clean
- **Terraform**: follow HashiCorp style, use `terraform fmt`
- **Python**: PEP 8, type hints appreciated
- **YAML**: 2-space indent, no tabs
- **Docker**: multi-stage builds where it makes sense, pin base image versions

---

## Reporting security issues

Please **don't open a public issue** for security vulnerabilities. See [`SECURITY.md`](SECURITY.md) if it exists in the repo, or contact me directly.
