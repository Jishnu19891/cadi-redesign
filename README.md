# CADI website redesign — HTML source for Figma import

## Pages
| File | Page |
|---|---|
| design-system.html | Tokens, type, buttons, cards — import this FIRST and turn into Figma styles/components |
| index.html | Home (12 sections, client-approved order) |
| integrations.html | API Integrations (was /integrations) |
| podcast.html | Podcast (was /podcast) |
| contact.html | Request a Demo (was the #contact anchor; now a page) |
| blog.html / blog-post.html | Blog index + post template (was blog.cadime.ai, WordPress) |
| security.html | Security & Trust page fronting trust.cadime.ai |
| get-started.html / login.html | App auth screens (app.cadime.ai) |
| terms-of-use.html | Terms of Use |
| data-processing-agreement.html | DPA |
| privacy-policy.html | Privacy Policy (text slot — live page embeds a third-party script) |
| cookie-policy.html | Cookie Policy (text slot — same) |

Shared: styles.css (all tokens in :root at the top), img/ (photos cropped from the client's reference deck — replace with licensed originals before launch).

## Importing into Figma (editable layers, not screenshots)
1. In Figma, open Resources → Plugins → search "html.to.design" (by ‹div›RIOTS) → Run.
2. Choose the **"HTML"** tab (or "URL" if you host this folder) and paste the contents of a page's .html file.
   - When pasting HTML, also paste styles.css inside a <style> tag in the <head> first, or host the folder (e.g. GitHub Pages / Netlify drop) and use the URL tab — URL mode is more reliable because images and fonts resolve.
3. Set viewport 1440 for desktop frames, 390 for mobile frames, then Import. Repeat per page.
4. Start with design-system.html: convert the colour swatches to colour styles, the type rows to text styles, and the button/card blocks to components. Then import the pages and swap their instances to those components.
5. Fonts: Archivo (variable, width axis) and Inter — both on Google Fonts, both available in Figma. Deel's own display face is Bagoss Condensed (commercial); Archivo at ~78–80% width is the stand-in.

## Local preview
Open any .html file directly in a browser; no build step.
