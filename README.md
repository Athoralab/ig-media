# ig-media

Public host for Athora Lab Instagram carousel and story slide images. Instagram's Graph API fetches images from public URLs, so rendered slides are committed here and served as raw links.

## Folder convention

One PNG per slide, in swipe order: `YYYYMMDD/slug/slide_1.png`, `slide_2.png`, and so on. Matches the local render folder `slides/YYYYMMDD/slug/`. slide_1 is the cover, the last slide is the follow card.

## Public URL

`https://raw.githubusercontent.com/Athoralab/ig-media/main/YYYYMMDD/slug/slide_1.png`

That raw link is written to Airtable (IG Image URLs) and passed to the Graph API as each carousel image. Uploaded by ig_upload.py at render time. Public repo, rendered slides only, no secrets.
