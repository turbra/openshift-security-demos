# OpenShift security demos

Interactive walkthroughs of network controls, project permissions, and an approved request-to-production operating model. Each demo is a standalone HTML file with embedded fonts and artwork.

## Choose a Demo

Open the [catalog](./index.html), or go directly to a demo:

| Demo | What it shows |
| --- | --- |
| [Network policy](./ocp-containment-demo-network-policy.html) | A compromised application's lateral connection is blocked while approved traffic continues. |
| [Self-provisioning](./ocp-containment-demo-self-provision.html) | Project creation supplies an entry point; a separate privilege-handling weakness supplies escalation. |
| [Operating model](./ocp-proj-req-to-prod.html) | Project approval, baseline provisioning, user access, and approved CI/CD deployment with separate runtime identities. |

Use each demo's playback controls or select a stage directly. Expand its technical details for assumptions, enforcement checks, and OpenShift documentation.

## Run Locally or Offline

Open `index.html` or any demo HTML file directly in a browser. No build, package installation, or external runtime assets are required. Documentation links require internet access.

To use a local static server, run this command from the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open [the local catalog](http://127.0.0.1:8000/). Stop the server with Ctrl+C.

For presentations, use GitHub's **Code → Download ZIP** or clone the repository, then keep a known-good copy of the HTML files. Open and test that copy offline before presenting. The repository is the maintained source.

## Publish with GitHub Pages

The site address is [turbra.github.io/openshift-security-demos](https://turbra.github.io/openshift-security-demos/). GitHub Pages is configured to publish `main` from `/(root)`, with HTTPS enforced.

To configure publication, go to **Repository Settings → Pages → Deploy from a branch → main → /(root) → Save**. Enable **Enforce HTTPS** when available. Keep the default GitHub Pages domain. The empty `.nojekyll` file bypasses Jekyll processing; no custom deployment workflow is needed.

Wait for the repository's **pages build and deployment** run to succeed. Check the HTTPS catalog and all three direct demo URLs, including a reload. Links must remain relative so they work under `/openshift-security-demos/` as well as offline.

Refer to GitHub's [publishing source guidance](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) and [HTTPS guidance](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https).

## Add a Demo

Preserve the framework and technical boundaries in [AGENTS.md](./AGENTS.md):

1. Add a standalone HTML file at the repository root. Reuse the established visual framework and unmodified official artwork, embedded fonts, and source license notices.
2. Add a catalog card with a concise description, a relative URL, and a distinct accessible link name. Update the demo table above.
3. Test the catalog and direct URL beneath `/openshift-security-demos/`, then open the HTML offline. Check desktop and narrow layouts, keyboard focus, and reduced motion.
4. Walk every stage. Check backward selection, restart, cumulative focus, fixed diagram positions, synchronized panels, and explicit denied or unavailable outcomes. Check the browser console and documentation links.
5. Publish through `main` and verify the deployed pages. Preserve existing demos unless a specific change is needed.

## Design References

Use the [Red Hat Technical Writing Style Guide, Design](https://stylepedia.net/style/#design) for concise organization, meaningful headings, labels, and terminology. Keep the established sentence-case catalog and demo titles. Use the [Red Hat logo standards](https://www.redhat.com/en/about/brand/standards/logo) and [product logo standards](https://www.redhat.com/en/about/brand/standards/product-logos) for the official OpenShift logo, proportions, and clear space.

Red Hat Display and Red Hat Text are embedded under the SIL Open Font License 1.1. Full font notices remain in the HTML source. Preserve them when copying assets.
