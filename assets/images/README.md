# Images

Store all image assets here that are referenced in your Markdown content.

## Folder Structure

Organise images into subfolders that mirror the content structure so that every image can be traced back to where it is used:

```
assets/images/
├── posts/     # Images used in blog posts
├── pages/     # Images used in static pages
└── shared/    # Shared images (logo, favicon, social-preview, etc.)
```

## Naming Convention

A consistent file name makes it easy to find, update and delete images as content evolves. Follow the rules below for every image you add.

### Post images

Mirror the post's own file name and append a short descriptor for the image role.

**Pattern:** `YYYY-MM-DD-post-slug-descriptor.ext`

| Part | Description | Example |
|---|---|---|
| `YYYY-MM-DD` | Publication date (same as the post file) | `2026-03-04` |
| `post-slug` | Kebab-case post title (same as the post file) | `hello-world` |
| `descriptor` | What the image shows or its role | `hero`, `diagram`, `screenshot-01` |
| `ext` | File extension in lower case | `.png`, `.jpg`, `.webp` |

**Examples:**
```
posts/2026-03-04-hello-world-hero.png
posts/2026-03-04-hello-world-screenshot-01.jpg
posts/2026-03-04-hello-world-architecture-diagram.svg
```

### Page images

Use the page slug followed by a short descriptor.

**Pattern:** `page-slug-descriptor.ext`

**Examples:**
```
pages/about-profile-photo.jpg
pages/about-team-banner.webp
pages/contact-map.png
```

### Shared images

Prefix with `shared-` so shared assets are instantly identifiable.

**Pattern:** `shared-descriptor.ext`

**Examples:**
```
shared/shared-logo.svg
shared/shared-favicon.png
shared/shared-social-preview.png
```

## Naming Rules

1. **Lower case only** – no uppercase letters anywhere in the file name.
2. **Kebab-case** – separate all words with hyphens (`-`); never use spaces or underscores.
3. **No special characters** – only letters, numbers, and hyphens.
4. **Descriptive descriptors** – use a noun or short noun phrase that describes the image role or subject (e.g. `hero`, `screenshot-01`, `profile-photo`).
5. **Lower-case extension** – always `.png`, `.jpg`, `.webp`, not `.PNG` or `.JPG`.

## Supported Formats

| Format | Use case |
|---|---|
| `.svg` | Logos, icons, diagrams (prefer SVG for vector artwork) |
| `.webp` | Photos and complex images (best compression, modern browsers) |
| `.png` | Screenshots, images that need transparency |
| `.jpg` / `.jpeg` | Photographs where WebP is not an option |
| `.gif` | Short animations only |

> **Tip:** Prefer `.webp` over `.jpg`/`.png` for photographs and UI screenshots to reduce page load time.

## Usage in Markdown

Reference images using paths relative to the Markdown file that contains them.

### From a post (`content/posts/YYYY-MM-DD-title.md`)

```markdown
![Hero image for Hello World post](../../assets/images/posts/2026-03-04-hello-world-hero.png)
```

### From a page (`content/pages/page-name.md`)

```markdown
![Profile photo](../../assets/images/pages/about-profile-photo.jpg)
```

### Shared image (from any content file)

```markdown
![Site logo](../../assets/images/shared/shared-logo.svg)
```

## Checklist When Adding an Image

- [ ] Placed in the correct subfolder (`posts/`, `pages/`, or `shared/`)
- [ ] File name follows the naming convention for its type
- [ ] File name is lower case with hyphens only
- [ ] File extension is lower case
- [ ] Alt text in the Markdown reference is descriptive and meaningful
- [ ] Image is appropriately sized and compressed before committing
