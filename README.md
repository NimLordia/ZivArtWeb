# ZivArtWeb

A portfolio website for multidisciplinary artist **Ziv Shaham**, built by **Nimrod Shaham** with HTML, CSS, and vanilla JavaScript.

**[View the live website](https://nimlordia.github.io/ZivArtWeb/)**

## About the project

The site brings Ziv's paper art, street art, video work, and theater productions together in one place. Visitors can browse artwork and production photographs, watch videos, and find the artist's biography and contact information.

## Features

- Separate sections for Paper Art, Street Art, Video Art, and Theater.
- Four theater productions, each with dedicated art, photo, and video pages.
- Image carousels with previous/next buttons and touch-swipe controls.
- Arrow-key navigation in selected theater galleries.
- A mobile hamburger menu and layouts that adapt to smaller screens.
- YouTube video integration.
- An artist biography, email link, and Instagram link.

## Built with

| Technology | Role |
| --- | --- |
| HTML | Page structure and content |
| CSS | Layout, styling, transitions, and responsive breakpoints |
| JavaScript | Navigation, gallery controls, touch gestures, and video-player integration |
| GitHub Pages | Static website hosting |
| YouTube | Video hosting and IFrame Player API |
| Cloudinary | Hosting for the site's favicon |

Gallery images and page backgrounds are stored in the repository's `Media/` directory and served with the site. Videos are hosted on YouTube; Cloudinary is used for the favicon.

## Run locally

No package installation or build step is required. To preview the site with Python 3:

1. Clone the repository:

   ```sh
   git clone https://github.com/NimLordia/ZivArtWeb.git
   cd ZivArtWeb
   ```

2. Start a local web server from the repository root:

   ```sh
   python -m http.server 8000 --bind 127.0.0.1
   ```

   On Windows, use `py -m http.server 8000 --bind 127.0.0.1` if Python is available through the `py` launcher.

3. Open [the local preview](http://127.0.0.1:8000/) in your browser.

You can also serve the repository with the VS Code Live Server extension. Start from `index.html`: the gallery navigation and close controls currently depend on the homepage's embedded content frame. An internet connection is needed for YouTube videos and the Cloudinary favicon.

## Project structure

| File or directory | Purpose |
| --- | --- |
| `index.html` | Homepage, main navigation, and content frame |
| `paper-art.html.html` | Paper art gallery; this is the current filename |
| `street-art.html` | Street art gallery |
| `video-art.html` | Video art gallery |
| `theater.html` | Theater production cards and gallery navigation |
| `AnDart.html`, `AnDphotos.html`, `AnDvideo.html` | Assembling and Disassembling |
| `DPart.html`, `DPphotos.html`, `DPvideo.html` | Debris Peasant |
| `MMart.html`, `MMphotos.html`, `MMvideo.html` | Meta Marionette |
| `MAart.html`, `MAphotos.html`, `MAvideo.html` | Morphous Androgynous |
| `contact.html` | Artist biography and contact links |
| `Media/` | Artwork, photographs, backgrounds, and supporting source material |

## Implementation notes

The site is a static frontend with no backend or build pipeline. The homepage loads section pages into an iframe, and styles and scripts are included directly in the HTML files. Changes to shared gallery behavior currently need to be applied across the relevant pages.

## Credits

- **Artist:** Ziv Shaham
- **Website development:** [Nimrod Shaham](https://github.com/NimLordia)
