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

## Customization

- Open `index.html` and look for `<!-- EDIT PLACEHOLDER: ... -->` comments to customize bio text, projects, hobbies, and travel plans.
- Update links in the "Where to Find Me" section (`#redirects`) to point directly to your preferred profiles.
- Colors, font sizing, and spacing can be adjusted via CSS custom properties at the top of `style.css`.
