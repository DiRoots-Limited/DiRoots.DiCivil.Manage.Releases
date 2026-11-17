# Documentation notes for DiRoots.DiCivil.Manage.Releases

Found while testing documentation PR previews on a replica of this repository (`DiRoots-Mauro/DiRoots.Sandbox.DiCivilManage.Releases`) and on the production site. None of these items is caused by the preview workflows; they are listed so they can be fixed separately.

## Broken images in production (1)

These references return 404 on the live site:
- `docs/pages/DrawingLayers/DL-Spreadsheet-Interface.md:71`: `../../../assets/images/GIFs/DL/DL-Add-LayerS.gif` - the file is named `assets/images/GIFs/DL/DL-Add-Layers.gif` (letter case differs); fix the link.

## Site size

The `gh-pages` branch holds about 570 MiB of files, almost all images and GIFs. GitHub Pages recommends repositories and published sites below 1 GB.
- Previews are not affected: they reuse the live images, so a preview of this site measured 40.7 MiB instead of 572 MiB.
- Suggested fix: compress the largest GIFs or convert them to MP4/WebM. Largest files: `assets/images/GIFs/DL/Spreadsheet-Interface-Features-Formula-Support.gif` (38.1 MiB), `assets/images/GIFs/DL/Formula-Support.gif` (38.0 MiB), `assets/images/GIFs/TOL/Complete-export-process.gif` (34.5 MiB), `assets/images/GIFs/DL/Complete-Import-Export-Workflow.gif` (29.5 MiB), `assets/images/GIFs/DL/Spreadsheet-Interface-Features-Visual-Change-Tracking.gif` (28.6 MiB).
