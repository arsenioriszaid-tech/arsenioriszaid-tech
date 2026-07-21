# Arsenio GitHub Profile — Design Specification

> A premium GitHub Profile README system inspired by the visual identities of Claude Code, Linear, Vercel, and Raycast. Dark, minimal, elegant, and built with intention.

---

## 1. Design Philosophy

The design system is rooted in four principles that define every decision in this profile:

| Principle | Description |
| :--- | :--- |
| **Calm** | No visual chaos. Every element earns its place. Generous spacing lets the content breathe. |
| **Precise** | Monospace typography, pixel-aligned borders, and a strict two-color palette. Nothing is accidental. |
| **Minimal** | Zero decorative noise. No rainbow colors, no unnecessary GIFs, no cringe developer clichés. |
| **Obsessed with craft** | Smooth SVG animations, terminal-inspired motifs, and a layout that feels like a beautifully designed IDE. |

---

## 2. Color Palette

The entire profile operates within a tightly controlled palette. Every hex value below is used across the SVG assets and is intended to remain consistent for maximum visual cohesion.

| Role | Hex Code | Usage |
| :--- | :--- | :--- |
| **Canvas** | `#0A0A0A` | Primary background for all sections and cards. |
| **Surface** | `#111111` | Subtle elevation for cards and hover states. |
| **Border** | `#1a1a1a` | Hairline borders to define structure. |
| **Accent** | `#D97706` | The signature orange. Used for cursors, highlights, icons, and animated elements. |
| **Primary Text** | `#FAFAFA` | Titles and primary headings. |
| **Secondary Text** | `#9CA3AF` | Body text and descriptions. |
| **Muted Text** | `#555555` | Labels, timestamps, and decorative elements. |
| **Dim Text** | `#333333` | Footer text and inactive states. |

---

## 3. Typography

| Property | Value |
| :--- | :--- |
| **Font Family** | `'SF Mono', 'Fira Code', 'JetBrains Mono', monospace` |
| **Title Size** | 32px bold |
| **Subtitle Size** | 13px, letter-spacing 3 |
| **Body Size** | 11–12px regular |
| **Label Size** | 9–10px, uppercase with letter-spacing 2 |
| **Font Color** | `#FAFAFA` (titles), `#9CA3AF` (body), `#D97706` (accent labels) |

The monospace font stack is universal across all sections to reinforce the terminal aesthetic. No serif or display fonts are used.

---

## 4. Folder Structure

```
arsenio/ (repository name must match GitHub username)
├── README.md
└── assets/
    ├── svg/
    │   ├── about.svg
    │   ├── banner.svg
    │   ├── contact.svg
    │   ├── contributions.svg
    │   ├── focus.svg
    │   ├── footer.svg
    │   ├── projects.svg
    │   ├── section-header.svg
    │   ├── separator.svg
    │   ├── stats.svg
    │   ├── status-bar.svg
    │   ├── tech-stack.svg
    │   └── typing.svg
    ├── previews/
    │   ├── about.png
    │   ├── banner.png
    │   ├── contact.png
    │   ├── contributions.png
    │   ├── focus.png
    │   ├── footer.png
    │   ├── projects.png
    │   ├── section-header.png
    │   ├── separator.png
    │   ├── stats.png
    │   ├── status-bar.png
    │   ├── tech-stack.png
    │   └── typing.png
    └── fonts/
        └── (optional: custom font files)
└── docs/
    └── SPECIFICATION.md
```

---

## 5. SVG Asset Inventory

Each SVG file serves a specific purpose in the profile layout. The table below describes each asset and its role.

| Asset | Width | Height | Purpose | Animation |
| :--- | :--- | :--- | :--- | :--- |
| `banner.svg` | 1200px | 200px | Hero section with name, role, and decorative elements | Cursor blink, accent line sweep, floating particles, scanline |
| `typing.svg` | 800px | 50px | Terminal-style typing animation with personal statement | Typewriter reveal, blinking cursor |
| `separator.svg` | 800px | 24px | Elegant divider between sections | Animated dot sweep, pulsing diamond |
| `about.svg` | 700px | 160px | Personal statement with quote styling | Static (decorative corner accents) |
| `focus.svg` | 700px | 120px | Current projects and learning areas | Pulsing status indicators |
| `tech-stack.svg` | 700px | 220px | Grid of technologies with categories | Subtle glow animation |
| `projects.svg` | 700px | 180px | Featured project cards with accent bars | Static layout |
| `stats.svg` | 700px | 140px | Static stats placeholder (dynamic widgets below) | Static layout |
| `contributions.svg` | 700px | 130px | Contribution graph visualization | Static grid |
| `contact.svg` | 600px | 60px | Social and website links | Border sweep animation |
| `footer.svg` | 800px | 60px | Minimal branded footer | Traveling dot animation |

---

## 6. Recommended Dynamic Widgets

The following GitHub widgets are recommended for dynamic data. All are configured to match the dark theme and orange accent.

### GitHub Stats Card

```
https://github-readme-stats.vercel.app/api?username=arsenio&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0A0A0A&title_color=D97706&text_color=9CA3AF&icon_color=D97706
```

### Streak Stats

```
https://github-readme-streak-stats.herokuapp.com/?user=arsenio&theme=tokyonight&hide_border=true&background=0A0A0A&stroke=1a1a1a&fire=D97706&currStreakNum=D97706&currStreakLabel=D97706
```

### Top Languages (Compact)

```
https://github-readme-stats.vercel.app/api/top-langs/?username=arsenio&layout=compact&theme=tokyonight&hide_border=true&bg_color=0A0A0A&title_color=D97706&text_color=9CA3AF
```

> Replace `arsenio` with your actual GitHub username in all widget URLs.

---

## 7. Icons

The design uses minimal Unicode and geometric symbols instead of icon libraries to maintain the monospace aesthetic. This avoids external dependencies and keeps the profile self-contained.

| Symbol | Usage |
| :--- | :--- |
| `▸` | Section header arrow indicator |
| `◆` | Project card bullet |
| `▌` | Typing cursor |
| `➜` | Terminal prompt / list item |
| `↗` | External link indicator |
| `●` | Status indicator (online) |
| `◆` | Decorative separator diamond |
| `⬡` | Tech stack item prefix |

---

## 8. Installation Steps

1. **Create the repository.** Go to GitHub and create a new public repository with the same name as your GitHub username (e.g., `github.com/arsenio/arsenio`).

2. **Clone the repository.** `git clone https://github.com/arsenio/arsenio.git`

3. **Copy the files.** Place the `README.md`, `assets/` directory, and `docs/` directory into the repository root.

4. **Customize the content.** Update the following in both the README and SVG files:
   - Replace `arsenio` with your actual GitHub username in all image URLs and widget URLs.
   - Update social links in `contact.svg` and the README contact section.
   - Modify project names and descriptions in `projects.svg`.
   - Adjust the tech stack in `tech-stack.svg` to match your actual skills.
   - Personalize the quote and description in `about.svg`.

5. **Commit and push.**
   ```bash
   git add .
   git commit -m "feat: add premium profile README"
   git push origin main
   ```

6. **Verify the profile.** Visit your GitHub profile page. The README should render automatically.

7. **Optional: Enable dark/light mode variants.** Use the `#gh-dark-mode-only` and `#gh-light-mode-only` HTML comments in the README if you want different assets for each theme.

---

## 9. Customization Guide

Every SVG file is pure SVG with inline styling. You can customize any element directly in the XML. Common customizations include:

- **Change accent color:** Replace all instances of `#D97706` with your preferred hex color across all SVG files.
- **Change font:** Update the `font-family` attribute in any SVG to use a different monospace stack.
- **Adjust animation speed:** Modify the `dur` attribute on any `<animate>` element to speed up or slow down effects.
- **Add new sections:** Create a new SVG file, upload it to `assets/svg/`, and reference it in `README.md` with the same pattern used by existing sections.

---

## 10. Performance Notes

| Consideration | Detail |
| :--- | :--- |
| **SVG Size** | All SVG files are under 5KB each, ensuring fast loading on GitHub. |
| **Render Limit** | GitHub renders SVGs up to ~10MB. All assets are well within limits. |
| **Animation Support** | GitHub supports SVG SMIL animations (`<animate>`) natively. |
| **CDN Caching** | GitHub may cache images for 10 minutes. Force-refresh by adding a query parameter (`?v=2`) if changes don't appear immediately. |
| **Image Path** | Use the `raw.githubusercontent.com` URL format: `https://raw.githubusercontent.com/USERNAME/REPO/main/PATH` |

---

## 11. Browser & Device Compatibility

| Platform | SVG Rendering | Animations |
| :--- | :--- | :--- |
| GitHub Web (Desktop) | Full support | Full SMIL animation support |
| GitHub Mobile App | Full support | Limited animation support (static fallback) |
| GitHub Dark Mode | Designed for dark mode | Color palette is dark-mode-native |
| GitHub Light Mode | Works with adjustments | Consider `#gh-light-mode-only` variants |

---

*Designed with precision. Built for developers who care about every pixel.*
