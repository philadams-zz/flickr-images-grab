flickr-images-grab
==================

Given a set of keywords, search the Flickr API, and download the images and
their associated metadata.

You'll need to edit `config.json.default` to include your Flickr API
key/secret, and edit `keywords.txt`.

Then grab search results (default 500 per keyword) via `python
flickr_images_grab.py --search`. And use those results (stored under `/search`)
to download the metadata and two images sizes for each photo: `python
flickr_images_grab.py --download` - these get dumped under
`/data/<keyword>.json` and `images/<keyword>/*.jpg`.
