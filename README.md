# iPhone Duo Case Studio

A static page — no build step, no server code. Upload this folder anywhere that serves files.

    index.html      the whole page (HTML, CSS and JS in one file)
    img/            Apple Store product photography
    .nojekyll       tells GitHub Pages to serve the files as-is

## Publishing

**Netlify Drop** — go to app.netlify.com/drop and drag this folder onto the page.
You get a live URL in a few seconds; no account needed to start.

**GitHub Pages** — create a repository, upload these files to the root of the
`main` branch, then Settings -> Pages -> Source: "Deploy from a branch",
branch `main`, folder `/ (root)`.

**Cloudflare Pages** — dash.cloudflare.com -> Workers & Pages -> Create ->
Pages -> "Upload assets", then drag this folder in.

Once it is live, the Share to X and Share to Threads buttons automatically link
to your URL instead of leaving the post link-less.

## Credit

Product photography and specifications are from the Apple Store and Apple
Newsroom and remain (c) Apple Inc. This page is an unofficial concept and is
not affiliated with or endorsed by Apple.
