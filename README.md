# Public Homepage

Public-safe fallback homepage powered by [Homer](https://github.com/bastienwirtz/homer) and deployed through GitHub Pages.

The intended routing is:

- **On Tailscale:** `home.ainatchi.me` resolves privately to the homelab Glance dashboard.
- **Off Tailscale:** public DNS resolves `home.ainatchi.me` to this GitHub Pages deployment.

## Editing the page

Edit `assets/config.yml` and push to `main`. GitHub Actions downloads the latest Homer release and deploys the resulting site automatically.

## GitHub Pages

In **Settings → Pages**:

1. Set **Source** to **GitHub Actions**.
2. Set the custom domain to `home.ainatchi.me`.
3. Configure the public DNS record GitHub requests.
