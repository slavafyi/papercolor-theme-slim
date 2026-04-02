# Agent Notes

## Fork Goal

- This fork modernizes `papercolor-theme-slim` for Neovim `0.12+`.
- Preserve the original PaperColorSlim palette and overall look in both dark and light variants.
- Prefer fixing missing or broken Neovim highlight coverage over redesigning the theme.

## Editing Rules

- Prefer new highlight links and reuse existing theme colors before adding new explicit color values.
- Do not change core palette choices unless needed to fix a real Neovim bug or prevent fallback to Neovim's default palette.
- Keep `colors/PaperColorSlim.vim` and `colors/PaperColorSlimLight.vim` structurally aligned.
- Target Neovim behavior, not Vim compatibility.

## Review Workflow

- When checking visual changes, prefer isolated `nvim --clean` runs so only the colorscheme source changes.

## Commits

- Use Conventional Commits.
- Keep the commit subject on a single line and at most 79 characters.
- Unless the user explicitly asks for it, do not add a commit body/description.
