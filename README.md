# PRODBYGOURD website

Upload the **contents** of this folder to any static website host. The included pages are Home, About, Press, Discography, Freelance, and Contact. The Store menu item points to Lemon Squeezy.

For local preview, run `python3 -m http.server 8000` from this folder and open `http://localhost:8000`. Do not open `index.html` directly as a file: internal links use site-root paths.

The contact forms use FormSubmit to send messages to `potenzageo23@gmail.com`. The inbox owner must verify the first FormSubmit activation email after a form submission; until then, delivery is not active. The site does not collect or store messages itself.

The footer uses search links for Apple Music, Spotify, and YouTube because exact artist profile URLs were not provided. Replace those with verified profile URLs if desired. Instagram and TikTok use the requested `prodbygourd` handle.

The audio players hide the browser's standard download control, but public audio cannot be made impossible to save or record. The five uploaded WAVs were encoded as 192 kbps MP3s for web playback. Original WAVs are not included in this ZIP.

This is a standalone website ZIP. Framer does not import it as an editable Framer project. You can host it on a static host or rebuild its layout in Framer.

The `tokyo club!` cover uses a compressed, muted, looping MP4 converted from George’s MOV file. The full-resolution MOV is not bundled to keep the site download manageable.

“natural light” by Vicky Gao uses the official Apple Music 30-second audio preview in the same track-card player as the other songs. A link opens the full track on Apple Music.

The homepage newsletter uses the supplied Kit embed. Kit controls subscription confirmations and campaign delivery; those settings must be enabled in the connected Kit account.

## Publish with GitHub Pages and prodbygourd.net

1. Upload the **contents** of this ZIP to the root of your GitHub repository. Keep the `CNAME` file and `.nojekyll` file at the repository root.
2. In the repository, open **Settings → Pages** and choose **Deploy from a branch**, `main`, `/ (root)`. Set **Custom domain** to `prodbygourd.net` and save.
3. At the domain's DNS provider, replace the old website A/AAAA records for `@` with these GitHub Pages A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`. If old AAAA records point to Framer, remove those too. Preserve MX and TXT records that handle email.
4. Create or update `www` as a CNAME pointing to **YOUR-GITHUB-USERNAME.github.io** (replace the placeholder with the actual account or organization hosting the repository; do not include the repository name). Remove any old `www` CNAME to Framer.
5. Back in **Settings → Pages**, wait for the DNS check and HTTPS certificate, then turn on **Enforce HTTPS**. `www.prodbygourd.net` should redirect to `prodbygourd.net`.

Do the DNS switch only after the GitHub Pages version is deployed and the GitHub username is known. DNS changes can take time to spread.

## Kit signup

The newsletter shows one email field and a Subscribe button. To make the subscriber immediately active without clicking a confirmation link, open Kit's form `93e6131007`, then **Settings → Confirmation Email → Auto-confirm new subscribers**. In the form's after-subscribe settings, replace its current “check your email to confirm” success text with a simple success message. Kit's account owner must make these settings in Kit; changing the website alone cannot change the form's confirmation requirement. Use Kit broadcasts or an automation to send future update emails.
