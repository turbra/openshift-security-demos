# Maintain the Demo Collection

The three existing demo HTML files are the authoritative visual and technical baseline. Keep their filenames, locations, embedded assets, font license notices, and standalone offline operation. Use plain HTML, CSS, and JavaScript; no build system, shared runtime extraction, or custom deployment workflow is needed.

## Preserve the Presentation

- Keep the complete topology visible from the first stage. Nodes, boundaries, and routes stay fixed as stages change.
- Derive cumulative focus from the selected stage: introduced sections stay clear; future sections soften to approximately 25% opacity and 1.5 px blur. Backward selection and restart must soften future sections again.
- Keep first reveal, active highlighting, and authorization results separate. Readable content does not imply an action can run. Avoid compounded focus in nested sections and preserve animation wrappers.
- Keep comparison panels synchronized. Preserve each demo's existing playback controller, stage selection, previous/next controls where present, restart, keyboard access, and reduced-motion support. Do not normalize controller behavior during hosting work.
- Make arrow source, destination, label, and enforcement point clear. Denied and unavailable paths must not animate as successful access.
- Keep blue protection, orange threat or successful unauthorized activity, and red denial with explicit labels or symbols.
- Keep the white canvas, readable Red Hat typography, restrained spacing, and exact official OpenShift logo asset, proportions, clear space, and existing transparent-canvas framing. Do not redraw or generate a substitute logo.
- Retain expandable technical explanations and relevant OpenShift documentation links.
- Keep embedded download controls, illustrative-demonstration boilerplate, style-guide footer links, visible font-credit footers, and shortcut-help footers absent. Put offline/source guidance in the README; retain licenses in source.

## Preserve the Technical Framing

- Network policy: preserve the attacker web client, external HTTPS endpoint, blue protected namespace, approved traffic, and blocked lateral connection. Keep the established title, subtitle, and takeaway. Claims apply to the shown policy and traffic; do not imply application repair or prevention of all exfiltration. Do not add PHP or unnecessary application-port/backend detail.
- Self-provisioning: distinguish the ordinary authenticated account from the operator/service account. Preserve initially limited permissions and the direct protected operation returning Forbidden. Keep project creation as the entry point and the separate Privilege-handling weakness as escalation, both visible in the main diagram. Custom-image builds are not a prerequisite. Qualify Potential cluster compromise by the exposed authority. Restriction only prevents this account from creating the project required by this path; it does not remove existing access or repair the weakness. Approved projects still require enforced permissions and secure operator behavior. No finding IDs, named vulnerable operators, exploit commands, payloads, or lab identifiers.
- Operating model: retain application ownership, environment/connectivity requirements, approval owners, project baseline, user-access approval, and approved CI/CD. Separate deployment from runtime identities. Preserve production without application-team project admin and the caveat that development project admin can deploy directly and change policies unless additional controls enforce restrictions. The project-request template covers that creation path; direct Namespace/Project automation must apply and verify the same baseline.
- Distinguish approval from enforcement and organizational configuration from product defaults. Verify changed technical claims against primary OpenShift documentation for the relevant release.

## Validate and Publish

Keep catalog links relative and demo link names distinct. Inspect desktop and narrow layouts, keyboard focus, console errors, offline files, cumulative focus, backward selection, restart, and reduced motion. Verify denied/unavailable outcomes and fixed geometry. For catalog/hosting-only changes, confirm the existing demos are byte-for-byte unchanged.

Publish through GitHub Pages using **Deploy from a branch → main → /(root)** with `.nojekyll` and HTTPS enforcement. Verify the actual HTTPS catalog and direct demo URLs before claiming publication. Keep workspace paths, preview addresses, credentials, and hosting metadata out of repository files. See the README for maintenance steps and required style/brand references.
