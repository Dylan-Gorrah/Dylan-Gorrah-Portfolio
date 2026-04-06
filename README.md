# Dylan Gorrah — Portfolio

A single-file HTML portfolio. No build tools, no npm, no config. Just open `index.html` and it works.

---

## File Structure

Set your project up exactly like this before opening anything in a browser:

```
your-portfolio-folder/
│
├── index.html              ← the portfolio (rename portfolio.html to this)
│
├── IMG/
│   └── profile.jpg         ← your profile photo goes here (see below)
│
└── CV/
    └── Dylan_Gorrah_Frontend_Developer.pdf  ← your CV PDF goes here
```

> **Tip:** The folder and file names are case-sensitive on Linux and most web servers. Use the exact names shown above.

---

## Step 1 — Add Your Profile Photo

1. Get a photo of yourself. A square crop works best — head and shoulders, clean background.
2. Rename the file to exactly: `profile.jpg`
3. Create a folder called `IMG` (uppercase) in the same folder as `index.html`
4. Drop `profile.jpg` inside the `IMG` folder

Then open `index.html`, find this comment near line 100:

```html
<!--
  ADD YOUR PHOTO: replace the <span> below with:
  <img src="IMG/profile.jpg" alt="Dylan Gorrah" />
  Full setup instructions in README.md
-->
<span class="profile-initials">DG</span>
```

Replace the `<span>` line with:

```html
<img src="IMG/profile.jpg" alt="Dylan Gorrah" />
```

Save the file and refresh your browser. Your photo will appear in the centre of the orbital.

### Photo tips
- Square images work best (e.g. 400x400px or 600x600px)
- Face centred in the frame — it crops to a circle
- File size under 500KB keeps load time fast
- Supports `.jpg`, `.jpeg`, `.png`, `.webp` — just make sure the filename matches what you put in the `src`

---

## Step 2 — Add Your CV PDF

1. Make sure your CV is saved as: `Dylan_Gorrah_Frontend_Developer.pdf`
2. Create a folder called `CV` in the same folder as `index.html`
3. Drop the PDF inside the `CV` folder

The Download CV button in the top right and the one inside the About panel will both link to this file automatically.

---

## Step 3 — Rename the HTML File

Rename `portfolio.html` to `index.html`. This is what web servers and GitHub Pages expect as the default page.

---

## Step 4 — Open It

Double-click `index.html` to open it in your browser. No server needed — it works offline too.

---

## Deploying Online

### GitHub Pages (free, recommended)

1. Create a new repo on GitHub — name it `dylan-gorrah.github.io` for a personal site, or anything for a project site
2. Upload all your files (index.html, IMG folder, CV folder) to the repo
3. Go to **Settings > Pages**
4. Set Source to `main` branch, root folder (`/`)
5. Click Save — your site will be live at `https://dylan-gorrah.github.io` within a minute or two

### Netlify (also free, very easy)

1. Go to [netlify.com](https://netlify.com) and log in
2. Drag your whole portfolio folder into the Netlify dashboard
3. Done — it gives you a URL instantly

### Vercel

1. Go to [vercel.com](https://vercel.com), connect your GitHub account
2. Import the repo
3. Deploy — live in about 30 seconds

---

## Customising

### Updating contact links
All links are in the JavaScript section at the bottom of `index.html`. Search for `wa.me`, `mailto`, `github.com`, or `linkedin.com` to find and update them.

### Adding or removing a project
Find the `const projects = [...]` array in the JavaScript section. Each project looks like this:

```js
{
  icon: 'bag',                      // icon key — see list below
  name: 'Project Name',
  tagline: 'One line description',
  desc: 'Longer description shown in the detail view.',
  tech: ['React', 'TypeScript'],    // tech stack tags
  url: 'https://yoursite.com',      // set to null if no link
  year: '2025',
},
```

Just copy one block, paste it in, and fill in your details.

### Available icon keys
These are the icons you can use for projects:

| Key        | Looks like          |
|------------|---------------------|
| `bookOpen` | Open book           |
| `utensils` | Fork and knife      |
| `heart`    | Heart               |
| `bag`      | Shopping bag        |
| `mapPin`   | Location pin        |
| `zap`      | Lightning bolt      |
| `fileText` | Document with lines |
| `bot`      | Robot face          |
| `globe`    | Globe               |
| `terminal` | Code terminal arrow |

### Changing the availability badge
Find this line and edit the text:

```html
<span class="avail"><span class="avail-dot"></span>Open to new opportunities</span>
```

Change it to whatever suits your current status — "Available for freelance", "Not currently available", etc.

### Changing colours
All colours are CSS variables at the top of the `<style>` block. The main ones are:

```css
--bg:    #F3E8DF;   /* warm sand background */
--gold:  #57595B;   /* accent colour for text and icons */
--txt:   #452829;   /* main text colour */
--green: #4a8c6a;   /* availability badge green */
```

---

## Tech Used (no installs required)

- **Google Fonts** — Cormorant Garamond + Outfit, loaded via CDN
- **Devicon** — Tech brand icons for the orbital, loaded via CDN
- **Lucide-style SVGs** — All UI icons are inline SVG, zero dependency
- Pure CSS animations for the orbit, entrance fades, and hover effects
- Vanilla JavaScript for panel open/close and project rendering

---

## Browser Support

Works in all modern browsers: Chrome, Firefox, Safari, Edge. No IE support — that's fine, nobody uses it.

---

## Questions?

Reach out via WhatsApp: 067 702 0221 — or email dylangorrah3@gmail.com
