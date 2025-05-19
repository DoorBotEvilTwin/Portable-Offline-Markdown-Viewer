# Portable Offline Markdown Viewer

Tired of searching for a truly **portable**, **offline**, and **functional** Markdown viewer that *just works*? So were we. This is a single HTML file solution (plus the `marked.js` library) that provides a clean, resizable, two-pane interface for pasting or typing Markdown and seeing a live preview.

**The Problem:** It's surprisingly difficult to find a simple, no-installation-required Markdown viewer that works locally without an internet connection, allows easy pasting of Markdown, and offers a resizable preview. Many existing solutions are overly complex, require Node.js, are part of larger editor suites, or simply don't work as advertised.

**This Solution:** This tool was created to fill that gap (after searching through dozens of so-called "offline markdown viewers" on GitHub, none of which worked as intended). It's lightweight, entirely client-side, and provides the core functionality needed for quick Markdown viewing and editing.

## Features

*   **Truly Portable:** Just one HTML file and one JavaScript file (`marked.min.js`). Drop them in a folder, and you're good to go.
*   **Fully Offline:** Once you have `marked.min.js` saved locally, no internet connection is required.
*   **Live Preview:** See your Markdown rendered as HTML in real-time as you type or paste.
*   **Resizable Panes:** A draggable vertical bar allows you to resize the input and preview panes. You can even shrink one almost completely to focus on the other.
*   **Direct Paste & View:** Easily paste Markdown content into the input area.
*   **Lightweight:** Minimal code, fast loading.
*   **GitHub Flavored Markdown (GFM) Support:** Leverages `marked.js` for robust Markdown parsing, including tables, fenced code blocks, etc.
*   **Basic Styling:** Includes sensible default styling for rendered Markdown, inspired by GitHub.
*   **No Installation, No Dependencies (beyond a browser):** Runs in any modern web browser.

## How to Use

1.  **Download `marked.min.js` (included):**
    *   Go to [https://cdn.jsdelivr.net/npm/marked/marked.min.js](https://cdn.jsdelivr.net/npm/marked/marked.min.js).
    *   Save the content of that page as a file named `marked.min.js`.
2.  **Download or Create `markdown_viewer.html`:**
    *   Download the `markdown_viewer.html` file from this repository.
    *   Alternatively, copy the HTML code provided.
3.  **Place Files Together:**
    *   Ensure both `markdown_viewer.html` and `marked.min.js` are in the **same folder**.
    ```
    your-folder/
    ├── markdown_viewer.html
    └── marked.min.js
    ```
4.  **Open in Browser:**
    *   Open `markdown_viewer.html` in your preferred web browser (e.g., Chrome, Firefox, Edge, Safari).

5.  **Using the Viewer:**
    *   **Input:** Paste or type your Markdown text into the left-hand pane (the `<textarea>`).
    *   **Preview:** The right-hand pane will automatically update with the rendered HTML.
    *   **Resize:** Click and drag the vertical bar between the two panes to adjust their widths.

## Why This Tool?

After countless attempts to find a simple, offline, portable Markdown viewer on GitHub and elsewhere, none seemed to fit the bill for a straightforward, resizable, paste-and-see experience. This tool was built out of that necessity – a ~300 line solution to a surprisingly common problem.

It's designed for anyone who needs to quickly view or draft Markdown without the overhead of a full IDE or a web-dependent service.

## Technical Details

*   Built with plain HTML, CSS, and JavaScript.
*   Uses the [marked.js](https://github.com/markedjs/marked) library for Markdown parsing.
    *   The `marked.min.js` file must be present locally for offline use.

## Contributing

Found a bug or have an improvement? Feel free to:
*   Open an issue.
*   Fork the repository and submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE.txt)