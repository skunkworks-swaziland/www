# Eswatini / Swaziland custom-domain cutover

Configured GitHub Pages CNAME: `www.skunkworks.sz`. This PR aligns the homepage canonical, Open Graph URL, JSON-LD and sitemap/robots to that *existing* CNAME. The approved Skunkworks **Swaziland** wordmark remains intact.

## Do not merge until all release gates pass
- [ ] Domain owner confirms `www.skunkworks.sz` is the approved primary.
- [ ] Authoritative DNS `www.skunkworks.sz CNAME skunkworks-swaziland.github.io` resolves publicly; no wildcard or conflicting records.
- [ ] Domain verified against `skunkworks-swaziland` organisation in GitHub Pages security controls.
- [ ] GitHub Pages Settings → Pages → Custom domain displays `www.skunkworks.sz`.
- [ ] HTTPS certificate issued and **Enforce HTTPS** available/enabled.
- [ ] A real `https://www.skunkworks.sz/` HTTP 200 page displays the Swaziland country wordmark and CSS.
- [ ] Update `skunkworks-africa/theme/countries.json` canonical in a coordinated release, then rerun cross-country smoke checks.

This PR is intentionally a **DNS-gated draft**. Publishing the new canonical before DNS works would advertise an inaccessible destination. No change to the CNAME itself is needed.
