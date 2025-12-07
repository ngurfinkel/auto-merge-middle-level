# halo-node-test

Test repository for auto-merge workflow validation - Level 2 (middle tier).

This repository demonstrates automatic PR creation and auto-merge functionality in a multi-tier setup.

## Purpose

- Contains `halo-auto-merge-test` as a submodule in `lib/halo-auto-merge-test`
- When the submodule is updated, this triggers a workflow that:
  1. Updates the submodule pointer in the parent repository (halo-node-buildroot-test)
  2. Creates an auto-PR with `(auto)` prefix
  3. Auto-merge is enabled automatically
  4. PR merges when all checks pass

## Part of Test Chain

halo-auto-merge-test → **halo-node-test** → halo-node-buildroot-test

