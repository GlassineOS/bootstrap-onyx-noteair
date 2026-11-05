# CLAUDE.md — GlassineOS/bootstrap-onyx-noteair

Bringing GlassineOS onto the Onyx Boox Note Air (see `README.md`). Empty so far.

- Nothing vendor-owned: no firmware, boot loader binaries, partition dumps or decompiler output. Steps that need a vendor file take it from the user's own device.
- A recipe that writes a partition states how to undo it, and what that undo depends on.
- Commits carry an `Assisted-by:` or `Co-Authored-By:` trailer. Never add
  `Signed-off-by`. Run `.glassine/org/scripts/safety-scan.sh --staged` before committing.
- Organization guidance for coding agents, including the project knowledge search
  (run `git submodule update --init` if the import below is missing):

@.glassine/org/AGENTS.md
