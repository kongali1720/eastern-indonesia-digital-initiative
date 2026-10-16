# Git Commit Signing Verification

## Purpose

Document the checks used to verify signed Git commits for this repository.

## Local verification

Inspect the latest commit signature:

    git show --show-signature --no-patch HEAD

Verify a specific commit:

    git verify-commit <commit-hash>

A successful local verification should report a valid signature.

## GitHub verification

After pushing a newly signed commit, inspect its entry on the GitHub
commit history page and confirm that GitHub displays the Verified label.

Local signature verification alone does not guarantee that GitHub will
display Verified.

## Security

- Never commit private SSH keys, access tokens, or passwords.
- Register the public signing key with GitHub under Signing keys.
- Keep authentication keys and signing keys separate where practical.
- Do not rewrite published history solely to change signature status.
