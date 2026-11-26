# Skills da Atomica — Pages delivery

This public repository hosts the client-side access shell and encrypted payload for the private `iarketinglabs/skills-da-atomica` source repository.

GitHub Pages is configured to deploy only `site/`, which must contain exactly `.nojekyll`, `content.enc`, and `index.html`. The workflow rejects extra files and validates the encrypted envelope before deployment. Never commit catalog metadata, skill documents, source packages, ZIPs, credentials, or decrypted build output here.

The `github-pages` environment is restricted to `main` and requires approval by `iarketinglabs` before each deployment. Review the staged files before approving a deployment.

The content is encrypted in the browser using AES-GCM and PBKDF2. The ciphertext is publicly downloadable and can be attacked offline; this is not server-side authentication.
