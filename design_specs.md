# Carousel Design Specifications

## Canvas

- Aspect ratio: 4:5
- Dimensions: 1080 × 1350 px

## Typography

- Typeface: Kefir Light
- Font file: `kefir-light.otf`
- Size: 36 px
- Weight: Light
- Italic style: No italic font is available yet. Use regular Kefir Light; do not simulate italics. The user will provide an italic font later.
- Letter spacing: -2 px
- Line height: approximately 32 px between baselines (tight spacing requested for this carousel style).
- Color: Warm cream (`#F8F1E1`)

## Text placement and image treatment

- Center every text block horizontally and vertically on the full slide canvas (for 1080x1350, center at x=540, y=675). Do not shift text to a side or safe area. Use line breaks to fit the centered block. If centering would cover a face or main subject, choose a different crop or image so both requirements are met.
- Keep faces and main subjects unobstructed.
- Add a subtle black (`#000000`) gradient behind the text when needed or requested for visibility. Inspect each slide yourself and adjust the gradient before delivery if the cream text is hard to read; do not wait for the user to flag contrast issues.

## Source Images

- Build a growing library from all supplied Chembarathi images. Add every new image to the library; image selection for a specific post is a separate later step.
- Save all supplied and newly added image copies in the project `assets/` folder.
- When new images are supplied, copy each one from its source location into `assets/`. Keep the original files unchanged.
- Give each library copy a clear filename based on its visible content or supplied context. Record the original filename and exact source path alongside the new library path.
- Record each image's original filename, exact source path, library copy path, and description in `assets/image_library.md`.
- Do not crop, resize, retouch, or otherwise alter an image when saving it to the library. Keep the full image as supplied.
- Do not alter or overwrite the original image files. Check each source image's EXIF orientation before cropping, and apply the orientation to the post-specific working copy before resizing.
- Render text and design treatments directly into each finished slide image.
- Keep finished, post-ready slide images in each post's `slides/` folder.
- Keep only finished slide images in each post's `slides/` folder. Do not save separate overlay or base files.
- Crop an image only in a separate post-specific working file when needed for the layout; never crop the original or library copy.
- Make image adjustments only on post-specific working copies; leave originals and library images unchanged, and deliver only the finished slide images.
