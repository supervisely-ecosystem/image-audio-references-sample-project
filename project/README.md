This project uses Supervisely JSON format for image projects.

## Structure

- `meta.json` — project meta, `"projectType": "images"`. No classes or tags: the project is unannotated.
- `ds0/img/` — 20 images
- `ds0/ann/` — one empty annotation per image, named `<image>.json`
- `ds0/meta/` — image metadata, named `<image>.json`. The `audio` key holds the audio references: a list of `{"url", "name", "mimeType"}`. The other keys are credits.

The recordings themselves are not in this archive. Each `url` points to a file in the `audio/` folder of the GitHub repository, so the player works on any instance that can reach `raw.githubusercontent.com`.

## Useful links

- [Audio references on images (Python SDK)](https://developer.supervisely.com/getting-started/python-sdk-tutorials/images/audio-references)
- [Supervisely JSON format](https://docs.supervisely.com/data-organization/00_ann_format_navi)
- [Supervisely Ecosystem](https://ecosystem.supervisely.com/)
