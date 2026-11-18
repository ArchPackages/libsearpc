# AGENTS.md

## Supply-chain checks for AUR updates

`libsearpc` is an AUR fork (`upstream` is
`https://aur.archlinux.org/libsearpc.git`). Before importing an upstream update
or pushing packaging changes:

- Review the AUR git history and diffs, not just the latest snapshot. Treat
  unexplained changes to source URLs, checksums, patches or `prepare()` /
  `package()` logic as a red flag.
- Confirm every source URL points at the documented upstream project, not a
  fork, personal mirror or lookalike domain.
- Download sources independently and compare hashes with checksums published
  by upstream; do not trust the hashes in the AUR `PKGBUILD` alone.
- Inspect patches, launchers and any `.install` file for shell hooks, network
  access or unexpected executables.
- Never accept new AUR checksums without repeating the upstream verification.
- Record what was verified in the commit message.
