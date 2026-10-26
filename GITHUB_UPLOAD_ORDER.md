# GitHub Upload Order — t2-metrics

1. Switch the repository to the `t2-metrics` branch.
2. Upload the contents of this package to the repository root.
3. Preserve the existing repository folders; do not replace unrelated files.
4. Commit message: `Complete T2 metrics and system quality evidence`
5. Run the local T2 evidence commands before opening the pull request.
6. Open a pull request from `t2-metrics` into `main`.
7. Ask the lead to review/merge; the team plan says only the lead merges to `main`.

Important: `dashboard/system-quality-section.html` is a drop-in implementation. Because the actual `project_citypulse.html` source was not available in this workspace, it is not automatically merged into that single HTML file. Integrate the section into the existing dashboard using the project's current data-layer object/API, then commit that integration in the same branch.
