# Sweety Birthday Website — GitHub Pages

This version loads media from repository files, not temporary browser uploads. Photos and music remain available after refresh and to all visitors.

## Add photos
1. Open `assets/photos/`.
2. Add your photos named `photo-01.jpg` through `photo-12.jpg`.
3. If filenames/extensions differ, edit `CONFIG.photos` in `index.html`.
4. Photo order follows the list; the first photo is also used in the scratch card.

Supported formats: JPG, JPEG, PNG, WEBP.

## Add background music
1. Put an MP3 in `assets/music/` named `our-song.mp3`.
2. Or change `music:'assets/music/our-song.mp3'` in `CONFIG`.
3. Edit `trackTitle` and `artist` too.
4. Visitors must press Play; browsers block automatic audio playback in many cases.

## Change birthday details
Edit the `CONFIG` object near the bottom of `index.html`:
- `birthday`: `YYYY-MM-DDTHH:MM:SS` (Nepal local time)
- `previousAge`, `newAge`: age values
- `name`: page title
- `trackTitle`, `artist`: music player labels
- `music`: music file path
- `photos`: image file paths

## Change written messages/name
In `index.html`, use Ctrl+F to search for `Sweety` and edit visible name text. Search for phrases such as `A wish from my heart`, `To my favourite girl`, `Happiest birthday`, and `You deserve the whole universe` to edit messages. Keep the HTML tags around the text.

## Publish with GitHub Pages
1. Create a repository, e.g. `sweety-birthday`.
2. Upload the contents of this folder to the repository root. Keep `index.html` and `assets/` at the root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main`, folder `/ (root)`, then Save.
6. Your site will publish at `https://YOUR-USERNAME.github.io/sweety-birthday/`.

After changing media/text, commit and push again. GitHub Pages will update the site.

**Privacy:** If the repository is public, anyone can view the website and download its photos/music. Do not upload private images you do not want public.
