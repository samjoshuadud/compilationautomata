## Cursor Cloud specific instructions

This is a static HTML website (no build system, no package manager, no backend). All computation is client-side JavaScript embedded in the HTML files.

### Running the application

Serve the files with any static HTTP server:

```
python3 -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

### Structure

- `index.html` — Landing/menu page
- `divisionalgo.html` — Division Algorithm
- `euclidean.html` — Euclidean Algorithm (GCD/LCM)
- `collatz.html` — Collatz Sequence
- `fibonacci.html` — Fibonacci Numbers
- `lucas.html` — Lucas Numbers
- `tribonacci.html` — Tribonacci Numbers

### UI template reference

All operation pages follow the same layout established by `euclidean.html`:
nav-row, page-header (eyebrow + h1 + subtitle), info-box, input fields, button-row, explain-toggle, output, steps-card.

### Testing

No automated test framework. Verify by opening each page in a browser, entering valid inputs, and confirming correct output. There is no linting or build step.
