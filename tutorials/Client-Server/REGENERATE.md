# Regenerating client-server.pdf

Source of truth is `client-server.html`. Edit it, then re-render:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf="$(pwd)/client-server.pdf" \
  "file://$(pwd)/client-server.html"
```

No toolchain to install — print CSS (`@page`, `break-inside: avoid`) is in the HTML.
