# AGENTS.md

## What this repo is

This is a personal index of useful GitHub repositories. It is NOT a software project:
there is no code to build, test, or lint. The deliverables are:

- `README.md` - the index: one bullet per repo, grouped under fixed headings
  (Skills, Tools, Video / Media, Tutorial), each link with a one-line description.
- `repos/` - shallow clones of every listed repo (gitignored, reference only).
- `graphify-out/` - knowledge graph output (gitignored).

## Rules

1. **Never commit `repos/` or `graphify-out/`.** They are covered by `.gitignore`;
   keep it that way.
2. **Adding a repo:** verify it exists first (`git ls-remote <url>`), clone it
   shallow (`git clone --depth 1 <url> repos/<basename>`), then add one bullet to
   the README under the heading that matches what the repo DOES, not its name.
3. **Descriptions must come from the repo's own README**, condensed to one line.
   Never invent a description for a repo you could not read; leave it undescribed.
   If a repo is dead/private, keep the link with a note - do not drop it.
4. **Dedupe:** check the URL is not already listed before adding. Basename
   collisions in `repos/` are resolved with a prefix (e.g. `vercel-skills`).
5. **Commit style:** short imperative message, e.g. "Tambah <repo-name>".
   Push to `main` after committing.
6. Reply to the user in Indonesian.
