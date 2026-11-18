# Code Scanner

A static, browser-based scanner for QR codes and common 1D/2D barcode formats. It can scan from a camera or decode a local image; decoded text stays in the browser, with copy and safe HTTP(S) link actions.

Included formats: QR Code, Data Matrix, Aztec, PDF417, MaxiCode, Code 128, Code 39, Code 93, Codabar, ITF, EAN-8, EAN-13, UPC-A, and UPC-E.

## Use on GitHub Pages

Publish this repository (or a folder containing `index.html`) with GitHub Pages, then open the published HTTPS page. Camera access requires HTTPS or `localhost`. The scanner library is loaded from unpkg, so an internet connection is needed to load it.

The scanner uses ZXing's multi-format decoder with its harder-search hint enabled. No decoder can guarantee every decorative, damaged, low-contrast, or unsupported code will scan; use a clear image, good lighting, and the full code including its quiet zone.
