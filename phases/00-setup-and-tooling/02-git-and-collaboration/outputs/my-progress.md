# Git collaboration exercise

This practice record keeps the Git lesson reproducible while preserving ongoing
environment setup work as separate changes.

- Existing clone: `KEYUR141/ai-engineering-from-scratch` on GitHub.
- Practice branch: `my-progress`.
- Root `.gitignore` already excludes `*.pt`, `*.pth`, and `*.safetensors`.
- Ignore rules verified with `git check-ignore --no-index -v`.
- Reviewed general history and history scoped to `phases/00-setup-and-tooling`.
- Inspected commit `5687a471`: it changes the development environment lesson's
  macOS setup guidance (one file, 12 insertions, two deletions).

Recheck the checkpoint rules from the repository root:

```bash
git check-ignore --no-index -v lesson-check.pt lesson-check.pth lesson-check.safetensors
git log -5 --oneline -- phases/00-setup-and-tooling
git show --stat 5687a471 -- phases/00-setup-and-tooling
```

Publishing requires a successful `git push -u origin my-progress`. A local commit
alone does not confirm the GitHub exercise is complete.
