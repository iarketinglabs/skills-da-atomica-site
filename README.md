# Skills da Atomica — Pages delivery

This public repository hosts the client-side access shell and encrypted payload for the private `iarketinglabs/skills-da-atomica` source repository.

GitHub Pages is configured to deploy only `site/`. That directory may contain the access page, public assets, `.nojekyll`, and encrypted content. Never commit catalog metadata, skill documents, source packages, ZIPs, credentials, or decrypted build output here.

The content is encrypted in the browser using AES-GCM and PBKDF2. The ciphertext is publicly downloadable and can be attacked offline; this is not server-side authentication.
