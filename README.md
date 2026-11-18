# Code Scanner

A static, browser-based scanner for QR codes and common 1D/2D barcode formats. It can scan from a camera or decode a local image; decoded text stays in the browser, with copy and safe HTTP(S) link actions.

QR results preserve UTF-8 text, including emoji. Images can be selected or dragged onto the preview, and the light/dark theme follows the device preference with a manual toggle.

Included formats: QR Code, Data Matrix, Aztec, PDF417, MaxiCode, Code 128, Code 39, Code 93, Codabar, ITF, EAN-8, EAN-13, UPC-A, and UPC-E.

On phones, live scanning requests the rear-facing camera and 720p video when available, and confirms a result in consecutive frames to reduce false detections. You can select another camera after granting camera permission.

## Use on GitHub Pages

Publish this repository (or a folder containing `index.html`) with GitHub Pages, then open the published HTTPS page. Camera access requires HTTPS or `localhost`. The scanning libraries are loaded from jsDelivr and unpkg, so an internet connection is needed to load them.

The live camera uses jsQR for QR codes and ZXing's multi-format decoder for QR codes and common barcodes, with its harder-search hint enabled. Image uploads use ZXing. No decoder can guarantee every decorative, damaged, low-contrast, or unsupported code will scan; use a clear image, good lighting, and the full code including its quiet zone.
