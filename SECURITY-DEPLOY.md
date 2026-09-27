# Security and deployment notes

- This portfolio is a static site. It has no account system, contact form, analytics, cookies, or server-side code.
- Styles, scripts, images, certificates, and documents load from this site. It does not request Google Fonts or other third-party page assets.
- Outbound links open the named service in a separate tab without access to the portfolio tab or a referrer URL.
- `_headers` sets a restrictive Content Security Policy and browser security headers. Netlify and Cloudflare Pages support this file; other hosts need the equivalent response headers configured in their dashboard or deployment config.
- Serve the site over HTTPS and enable the host's HTTPS redirect. Security headers are not applied when opening `index.html` as a local `file://` URL.
- Email, phone number, social profiles, and the downloadable resume are public information on the site. Remove any detail you do not want visitors to see before publishing.
