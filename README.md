# Contour Explorer

Standalone experimental explorer for the Contour braided cup device. Current model: `contour-cup-0.4`.

Serve this directory with `python3 -m http.server 8765 --bind 127.0.0.1` and visit http://127.0.0.1:8765/contour.html (HTTP is required for the local Three.js modules). No build step. Vendored Three.js r170 lives under `vendor/` (MIT; see `vendor/README.md`). The Simulation panel shows a 2D meridional section beside a 3D solid-of-revolution view of the same synthetic geometry.

Run geometry tests from this directory with `node tests/contour.test.cjs`.

- [Model documentation](CONTOUR.md)
- [Future calibration protocol](CALIBRATION.md)
- [AngioSeg deployment prompt](DEPLOY_CONTOUR_PROMPT.md)
- [Device data request](docs/contour_neurovascular_system_data_request.docx)

The optional document generator `scripts/build_contour_data_request.py` requires Python, python-docx, Pillow and the font paths documented in its source.

Synthetic research prototype, not validated for clinical use. Excessive elongation remains unresolved. Not affiliated with, sponsored by or endorsed by Stryker or Medtronic. No clinical data belong in this public repository.

See [PROVENANCE.md](PROVENANCE.md) for migration and attribution. No open-source licence has been granted for this standalone project yet.
