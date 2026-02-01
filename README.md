# Will you be my Valentine? 💕

A simple, cute Valentine’s page with your photos and a Yes/No button.

## What’s included

- **index.html** – Single page with 3 photos, cute messages, and “Will you be my Valentine?” with Yes/No
- **photo1.jpg, photo2.jpg, photo3.jpg** – Your three photos (converted from HEIC)

## Host it so she can open the link

### Option 1: Netlify Drop (easiest)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag the **entire `vday` folder** (with `index.html` and `photo1.jpg`, `photo2.jpg`, `photo3.jpg` inside) onto the page
3. Netlify gives you a link like `https://random-name-123.netlify.app` — send her that link

### Option 2: GitHub Pages

1. Create a new repo on GitHub, then push this folder (with `index.html` and the 3 JPGs)
2. In the repo: **Settings → Pages → Source**: Deploy from branch, main, `/ (root)`, Save
3. Your site will be at `https://yourusername.github.io/repo-name/`

### Option 3: Open locally

Double-click `index.html` or run:

```bash
open index.html
```

She can use it on her phone or computer; the page works on both.

---

## HEIC → JPG (browsers can’t use HEIC)

Your three HEIC files are already converted to **photo1.jpg**, **photo2.jpg**, **photo3.jpg**. The page uses those JPGs.

To convert again (e.g. after replacing the HEIC files), on Mac in Terminal from the `vday` folder run:

```bash
sips -s format jpeg -s formatOptions 90 "69439071423__610F2D10-4E8B-4867-889E-C26F407927F3.HEIC" --out photo1.jpg
sips -s format jpeg -s formatOptions 90 "IMG_3510.HEIC" --out photo2.jpg
sips -s format jpeg -s formatOptions 90 "IMG_4508.HEIC" --out photo3.jpg
```

If you use different HEIC filenames, change the quoted names above and the output names to match what `index.html` expects (`photo1.jpg`, `photo2.jpg`, `photo3.jpg`).
