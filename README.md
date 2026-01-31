# ModernPDF

**This project is a fork of [Kevin Bryan's ModernPDF](https://github.com/kevincure/ModernPDF).** All credit for the core PDF viewer and annotation functionality goes to Kevin Bryan. You can find more of his projects at http://www.kevinbryanecon.com/tools.html.

This fork adds **link hover preview** functionality: when you hover over internal links (like footnote references, equation citations, or cross-references), a preview of the destination content appears in a tooltip. For external links, the URL is displayed on hover.

---

ModernPDF is an ultralightweight PDF reader that supports just enough annotation tools for quick markups. Load a document, drop text or comment pins, sign documents, and read.

**Chrome Extension:** ModernPDF is designed as a Chrome extension. While it may work in other Chromium-based browsers (Edge, Brave, Opera), it is not compatible with Firefox or Safari, which use different extension architectures.

## Install as a Chrome or Edge extension
1. Clone or download this repository to your machine and note the folder location (any folder is fine - just make sure nothing else but these files are in the folder).
2. In **Google Chrome**, open `chrome://extensions`, toggle **Developer mode** on, then click **Load unpacked** and choose the folder. In **Microsoft Edge**, open `edge://extensions`, enable **Developer mode**, and select **Load unpacked** to pick the same folder.
3. (Recommended) After loading, enable **Allow access to file URLs** in the extension card if you plan to open local PDFs from disk.
4. The ModernPDF action button toggles interception on/off. Leave it **ON** for automatic PDF replacement in the custom viewer.

## Workflow
- PDFs will automatically open from the web. If you want to use this for local PDFs, just select Chrome/Edge as the target for PDFs to open. The **Download** button saves a copy to your computer.
- Use the person icon to set your **name and signature**; both values persist between sessions.
- Press 'a' to add a text **annotation**. You can click on it later to edit.
- Press 's' to add your **signature**. You can shrink or expand it.
- Press 'm" to add a **comment**.  You can reply.  The user name chosen in identity is who the comment will appear linked to.
- Press 't' to **select text**. With any text highlighted with your cursor, you can press 'h' to add a permanent yellow **highlight** or 'x' for **strikethrough**.

## Navigation & Layout
- **Arrow keys**: Left/Right change pages, Up/Down scroll the current page.
- '+' and '-' zoom in and out. 'w' makes the page **full width**. '1' reverts to 100% zoom, 'r' toggles **reader mode** in full screen.
- You can click on the page number to jump to a page.
- Ctrl-f jumps to the 'find' bar. Press enter to search.

## Link Hover Preview (Fork Feature)
- **Internal links** (footnotes, equation references, cross-references): Hover over any internal link to see a rendered preview of the destination content. This is useful for reading academic papers where you want to quickly glance at a footnote or equation without losing your place.
- **External links**: Hover to see the full URL before clicking.

This is all deliberately minimal. Rendering is based on pdfjs.
- Signatures are draggable and resizable once placed; use the corner handle or reopen the identity dialog to redraw them at any time.

