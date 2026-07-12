# Tailwind CSS Demo

A minimal Tailwind CSS demo project with an `index.html` page and `style.css`.

## Project files

- `index.html` - sample page using Tailwind utility classes
- `style.css` - stylesheet for the project
- `package.json` - project dependencies

## Installed dependencies

This project currently uses:

- `tailwindcss@^4.3.2`
- `vite@^8.1.4`
- `postcss@^8.5.16`
- `autoprefixer@^10.5.2`

## Run locally

If you want to preview the page without a build step, open `index.html` directly in your browser.

## Build with Tailwind v4

Tailwind v4 does not use `init` and does not include a `tailwindcss init -p` command.

To build the CSS from `style.css` into `output.css`:

```powershell
npm install
npx @tailwindcss/cli build --input style.css --output output.css
```

Then update `index.html` to reference `output.css` instead of `style.css` if you want the processed file.

## Alternative: use Tailwind v3 style workflow

If you prefer the classic `tailwindcss init -p` workflow, install Tailwind v3:

```powershell
npm install -D tailwindcss@3 postcss autoprefixer
npx tailwindcss init -p
```

## Notes

- This repo is a small static demo, so a browser preview is the fastest way to check your work.
- If you use Vite, add scripts or a Vite config file to run a local dev server.
