# Birthday Website - Personalisation And Publishing Guide

This is a simple static website. There is no build step, no backend, and no coding setup required.

## Folder Structure

```text
birthday-website/
|-- index.html          Main birthday journey
|-- destinations.html   Travel dreams page
|-- images/             Put her photos here
|   |-- destinations/   Downloaded travel destination images
|-- README.md           This guide
```

## What You Need To Change

Open `index.html` and `destinations.html` in VS Code or any text editor.

Search for this exact phrase:

```text
UPDATE THIS PLACEHOLDER HERE
```

Every place you should personalise is marked with that comment.

Main things to update:

- Her name
- Her birthday date
- The opening line
- The letter/message
- Your name/signature
- Reasons you adore her
- Spotify playlist embed link
- Her photos
- Optional travel page text/images

## Adding Her Photos

1. Put her photos inside the `images/` folder.
2. Rename them with simple names:

```text
photo-1.jpg
photo-2.jpg
photo-3.jpg
```

Avoid spaces in filenames.

Good:

```text
her-smile.jpg
photo-1.jpg
birthday-photo.webp
```

Avoid:

```text
her smile.jpg
IMG 2026 final copy.jpg
```

3. In `index.html`, search for `Add photo 1`.
4. Replace the placeholder block:

```html
<div class="photo"><div class="placeholder">Add photo 1</div></div>
```

with:

```html
<div class="photo">
  <img src="images/photo-1.jpg" alt="Her smiling">
</div>
```

Repeat for the other photo placeholders.

Supported formats: `.jpg`, `.jpeg`, `.png`, `.webp`.

## Destination Images

The travel page uses local images stored in:

```text
images/destinations/
```

Each place has three images, for example:

```text
paris-1.jpg
paris-2.jpg
paris-3.jpg
```

If you want to replace a destination image, use the same filename and overwrite the file.

## Adding The Spotify Playlist

1. Open Spotify.
2. Open the playlist.
3. Click the three dots menu.
4. Choose `Share`.
5. Choose `Embed playlist`.
6. Copy the URL inside `src="..."`.
7. In `index.html`, search for `Spotify playlist embed URL`.
8. Replace the current `iframe src` URL with your playlist embed URL.

Only replace the URL, not the full iframe unless you are comfortable doing that.

## How The Locked Journey Works

The website is intentionally gated:

- She first has to open the birthday page.
- She must click the correct funny button.
- She must solve the sliding puzzle to unlock the gallery.
- She must answer the riddle to unlock the Spotify playlist.
- She can open the travel dreams page from the playlist section.
- She must finish the memory game to unlock the ending.

This works on phones and desktops.

## Testing Locally

The easiest test:

1. Double-click `index.html`.
2. It will open in your browser.
3. Try the full flow on desktop.
4. Also test it on a phone-sized browser window.

If an image does not show, check:

- The file is inside `images/`
- The filename matches exactly
- The extension is correct, for example `.jpg` vs `.jpeg`
- There are no spaces in the filename

## Publishing For Free - Netlify

Recommended because it is easiest.

1. Go to [Netlify](https://www.netlify.com/).
2. Create a free account.
3. On the dashboard, choose `Add new site`.
4. Choose `Deploy manually` or drag-and-drop deployment.
5. Drag the full `birthday-website` folder into Netlify.
6. Netlify will give you a link like:

```text
https://beautiful-name-123.netlify.app
```

7. You can rename the site in `Site configuration` if you want a nicer URL.

Whenever you edit the website later, upload the folder again to redeploy.

## Publishing For Free - GitHub Pages

Use this if you are comfortable with GitHub.

1. Create a GitHub account.
2. Create a new public repository, for example `birthday-website`.
3. Upload these files and folders:

```text
index.html
destinations.html
images/
README.md
```

4. Go to repository `Settings`.
5. Open `Pages`.
6. Under `Build and deployment`, choose:

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

7. GitHub will give you a link like:

```text
https://yourusername.github.io/birthday-website/
```

## Privacy Note

Free Netlify and GitHub Pages links are public if someone has the URL. They are usually not discovered randomly, but do not upload private photos unless both people are comfortable with that.

For maximum privacy, use a paid password-protected option or share only with the intended person.

## Quick Final Checklist

- Replace all `UPDATE THIS PLACEHOLDER HERE` items.
- Add real photos to `images/`.
- Replace the Spotify playlist link.
- Open `index.html` and complete the full flow once.
- Open `destinations.html` once.
- Upload the full folder to Netlify.

That is it. No server required.
