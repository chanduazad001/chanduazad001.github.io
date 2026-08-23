# chanduazad001.github.io

Personal hub page — links out to each lab/domain repo, published at the
GitHub Pages user-site root.

**Published site:** https://chanduazad001.github.io/

## Structure

This is a single static `index.html`, deliberately dependency-free (no
build step, no framework, no external CDN calls) — it only needs to list
labs and stay up. Each lab is its own repo with its own mkdocs site,
published as a GitHub Pages *project* site
(`chanduazad001.github.io/<repo>/`):

- [architecture-lab](https://github.com/chanduazad001/architecture-lab) — Cloud architecture, platform engineering, system design
- [cybersecurity-architecture-lab](https://github.com/chanduazad001/cybersecurity-architecture-lab) — Application, cloud, and enterprise security architecture

To add a new lab: build/publish the lab's own repo first, then add one
card to the `<section id="labs">` block in `index.html` here.

## Publishing

No GitHub Actions workflow — this repo is a user-site repo
(`<username>.github.io`), so GitHub Pages serves `index.html` directly
from the `master` branch root once **Settings → Pages → Source** is set
to "Deploy from a branch" / `master` / `/ (root)`. `.nojekyll` disables
the default Jekyll processing step since this is plain HTML.

## License

See [LICENSE](LICENSE).
