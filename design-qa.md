# BOOLE hero image design QA

- Source visual truth: `C:\Users\higes\.codex\codex-remote-attachments\01a0bc41-6b51-7fe1-8348-b812c63ed0dc\D50E7C8F-5829-4254-9428-CCB5442FE066\1-写真1.jpg`
- Implementation: `http://127.0.0.1:8000/about.html?v=interior1`
- Implementation screenshot: Codex in-app Browser capture for tab 4 (inline task artifact; the browser tool does not expose a filesystem path)
- Viewport: 390 × 844 CSS px, device pixel ratio 1
- Source pixels: 591 × 1280, including iPhone browser chrome
- Implementation pixels: 390 × 844, browser content only
- Normalization: compared the source page content below its browser chrome against the implementation content viewport
- State: page top after entrance transition

## Full-view comparison evidence

The original mobile hero used a low-contrast 3D render that visually dissolved into the warm-white background. The revised hero keeps the established type hierarchy and replaces that weak visual anchor with a portrait architectural image based on BOOLE's existing salon model. The blackboard, brass light, antique clock, pale wood counter, standing mirror, and barber chair now provide a high-contrast focal point and connect the editorial page to the 3D entrance.

## Focused region comparison evidence

The focused hero-image region was checked at mobile, tablet (834 × 1112), and desktop (1280 × 720). The generated image remains sharp at all three sizes. On mobile, the crop retains the pendant light, chalkboard wordmark, mirror, counter, and chair. The body copy remains on the paper background and the Descend control stays legible over the dark image.

## Required fidelity surfaces

- Fonts and typography: unchanged from the accepted BOOLE editorial system; the new image does not disturb headline wrapping or optical hierarchy.
- Spacing and layout rhythm: desktop remains an asymmetrical text/image composition; mobile uses the lower 37% of the hero for the image, preserving a readable text block above.
- Colors and visual tokens: warm white, charcoal, aged brass, pale wood, and ink remain consistent with the existing tokens.
- Image quality and asset fidelity: the 1024 × 1536 source is delivered as a 180 KB WebP, with a responsive editorial crop and descriptive alt text.
- Copy and content: unchanged; the visible `INTERIOR / B1F` caption clarifies the role of the image without adding promotional copy.

## Comparison history

1. Initial implementation used a 43% mobile image height. P2: the final lines of the introduction overlapped the image transition and lost contrast.
2. Reduced the mobile image height to 40%. P2 remained at the final line on a 390 × 844 viewport.
3. Reduced the image height to 37%. Post-fix evidence shows the full introduction on warm white with the image beginning below it; no P0/P1/P2 findings remain.

## Follow-up polish

- P3: replace the generated architectural image with an equivalent real salon photograph when BOOLE can provide one; the HTML and crop are ready for a direct asset swap.

## Verification

- Hero asset loaded: 1024 × 1536, complete, non-zero natural dimensions.
- Mobile, tablet, and desktop compositions checked in the in-app Browser.
- Console warnings/errors: none.
- Accessible image description: present.
- Existing reduced-motion behavior is unchanged; parallax remains disabled when reduced motion is requested.

final result: passed
