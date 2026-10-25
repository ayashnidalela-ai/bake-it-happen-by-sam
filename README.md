# Bake It Happen by Sam

A multi-page website for a home bakery in Dwarka, Delhi. Plain HTML, CSS and vanilla JavaScript, with no build step.

## Folder structure
```
index.html  menu.html  our-story.html  contact.html
css/style.css        all styling and colour variables (top of file)
js/script.js         contact constants, menu data, nav, form, animations
assets/images/       your photographs + placeholder.svg
```

## Preview locally
Open `index.html` in a browser. To test like a server: `python3 -m http.server` in this folder, then visit http://localhost:8000.

## Add your photographs
Put your photos in `assets/images/` using these exact filenames (or edit the `src` in the HTML):
`hero.jpg`, `cakes.jpg`, `cupcakes.jpg`, `cookies.jpg`, `treats.jpg`, `story.jpg`, `gallery-1.jpg`, `gallery-2.jpg`, `gallery-3.jpg`.
Until a file exists, `placeholder.svg` is shown instead. Adjust cropping with `object-position` (e.g. `style="object-position:center 30%"`).

## Edit products
Open `js/script.js` and edit the `MENU` array. Each item has `name`, `description`, `price` (leave `''` for "Price on request"), `image`, and `demo`. Remove `demo: true` once an item is real. The current items are **demonstration content only**.

## Contact details
Set in the `CONTACT` constant at the top of `js/script.js`. The static links in the HTML (footer, contact page, Instagram buttons) use the same values; search for `princy280206` or `8858850501` if you change them.

## Contact form
There is no backend. The form validates input, then opens a `mailto:` draft. The visitor must press Send in their email app.

## Deploy on GitHub Pages
1. Create a repository and upload all files, keeping the folder structure.
2. Go to Settings, then Pages. Under Source choose "Deploy from a branch", pick `main` and `/ (root)`, then Save.
3. After a minute your site is live at `https://<username>.github.io/<repository>/`.
