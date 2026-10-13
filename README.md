# frontage

A minimalist, aesthetic personal front page designed to serve as an online outpost and redirection hub. Ready with placeholders for personal bio, projects, hobbies, travel plans, and external profile links.

## Aesthetic & Design

- **Dark Screen Canvas**: Deep obsidian/charcoal dark tones (`#0a0d14`) optimized for contrast and readability.
- **Tasteful Accents**:
  - **Green**: Status badges, terminal outputs, and live indicator accents.
  - **Gold**: Brand highlights, titles, and call-to-action buttons.
  - **Violet**: Creative tags, category badges, and subtle glows.
  - **Blue**: System tags, link hovers, and ambient atmosphere.
  - **Organic Red Splotches**: Fluid, multi-toned crimson and ruby SVG gradient splotches with soft blurs drifting gently across the background.

## Features

- **About**: Bio summary with quick highlight cards (Technology, Exploration, Curiosity).
- **Projects**: Showcase grid with tags, status pills, and external repository/demo links.
- **Hobbies**: Visual cards for outdoor adventures, culinary/coffee pursuits, reading, and photography.
- **Travel Plans**: Categorized timeline of upcoming journeys, planning phases, and travel bucket list.
- **Online Redirects**: Quick directory linking to GitHub, LinkedIn, Email, and social presence.
- **Zero Dependencies**: Pure HTML5 and modern CSS (fully responsive, mobile-friendly, accessible).

## Local Preview

To preview the website locally on your computer:

```bash
# Using Python
python3 -m http.server 8080

# Or open directly in your web browser
open index.html
```

Then visit `http://localhost:8080` in your web browser.

## Hosting on GitHub Pages with Namecheap DNS

This static site can be published from the repository root. In GitHub, open
**Settings → Pages**, select **Deploy from a branch**, then choose `main` and
`/(root)`. After the first deployment, the default URL is
`https://tyson-dowd.github.io/frontage/`. New commits to `main` will publish
automatically.

To use a Namecheap domain for this site:

1. Enable GitHub Pages as described above.
2. In Namecheap, open **Domain List → Manage → Advanced DNS** and add:
   - For an apex domain (`example.com`), four **A** records with host `@` and
     values `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and
     `185.199.111.153`.
   - For `www.example.com`, a **CNAME** record with host `www` and value
     `tyson-dowd.github.io`.
3. In GitHub **Settings → Pages**, set the custom domain to the hostname you
   want to use and enable **Enforce HTTPS** once it becomes available. Add that
   exact hostname as the sole line in a root-level `CNAME` file in this
   repository.
4. If you use a different hostname, update the DNS records accordingly. Allow
   time for DNS propagation and HTTPS certificate provisioning to complete.

Do not use Namecheap's **URL Redirect Record** for this setup: it redirects
visitors to another URL rather than pointing the domain at this hosted site.
Use DNS records to connect the domain to GitHub Pages. The domain is not yet
specified, so this repository intentionally has no `CNAME` file; add it after
choosing the domain.

## Customization

- Open `index.html` and look for `<!-- EDIT PLACEHOLDER: ... -->` comments to customize bio text, projects, hobbies, and travel plans.
- Update links in the "Where to Find Me" section (`#redirects`) to point directly to your preferred profiles.
- Colors, font sizing, and spacing can be adjusted via CSS custom properties at the top of `style.css`.
