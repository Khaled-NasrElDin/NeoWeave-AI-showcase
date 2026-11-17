# Public-showcase security checklist

## Before publication

- [ ] Keep the complete application and its Git history in a separate **private** repository.
- [ ] Do **not** clone, fork, mirror, or copy `.git/` from the original application into this showcase.
- [ ] Start this showcase from an entirely fresh Git history.
- [ ] Review every file, including SVG, HTML comments, image metadata, and linked URLs.
- [ ] Confirm no credentials, tokens, API keys, customer data, real ERP payloads, database files, logs, stack traces, sensitive infrastructure URLs, or private addresses exist.
- [ ] Confirm no original backend Python, implementation-specific JavaScript, SQL schema, mapping contracts, recovery algorithms, tests, or source maps have been copied.
- [ ] Recheck marketing claims against the *current* Codex worktree and verified tests.
- [ ] Inspect the Git commit history before publishing.
- [ ] Check that links do not reveal a private GitHub repository or service endpoint.

## What visitors can still copy

Everything in a **public** GitHub repository is readable and downloadable, including this static HTML/CSS, SVG diagrams, and documentation. This template protects the private engine by not including it. It is **not** copy protection, a DRM mechanism, or a guarantee against imitation.

No license is provided for the project content. That alone is not a technical barrier to downloading it. Consult a qualified IP professional before relying on copyright, trademark, or trade-secret protections for commercial strategy.

## Prior public disclosure

If source code was previously published, changing a repository to private, deleting files, or rewriting Git history cannot retract copies already downloaded, indexed, cached, or forked. Review old exposure separately and rotate any credentials that may have been committed.

## Publishing this project

1. Visit https://github.com/new and create an **empty** public repository named `NeoWeave-AI-showcase` under `Khaled-NasrElDin`. Do not initialize it with a README; the package already contains one.
2. Extract this showcase archive to its own local folder, **not inside the private repository**.
3. Review and approve the full set of files.
4. In that folder, run:

   ```bash
   git init -b main
   git add README.md TECHNICAL_OVERVIEW.md SECURITY_AND_PUBLICATION.md .gitignore docs
   git commit -m "Publish code-free NeoWeave AI showcase"
   git remote add origin https://github.com/Khaled-NasrElDin/NeoWeave-AI-showcase.git
   git push -u origin main
   ```

5. Enable GitHub Pages from `main` / `docs` in **Settings → Pages**.
6. Preview the live site before adding its link to LinkedIn.

Do not push a ZIP file into GitHub and expect GitHub Pages to extract it. Extract the package first and commit the files.
