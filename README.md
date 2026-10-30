# SIwave Stackup Studio

Standalone HTML tool for PCB stackup editing. Open index.html in a browser or use the GitHub Pages website. No installation, server, account, or external page dependency is required. This is an independent helper, not an Ansys product.

v2.9 commits a copper-count change when input is finished (on change/blur), keeps Apply and Enter, and adds an immediate16-copper quick selection that preserves existing layer data. Reductions still require confirmation and support undo. All detail rows expand in the page; preview uses an explicit expand/collapse button instead of an internal vertical scrollbar. Phone-width tables still scroll horizontally to keep columns readable.

The SIwave table column order, material-derived electrical values, selectable metal-layer dielectric fill, and local preview colors remain available. Basic editing and original generic presets remain intact; no company-specific stackup photo or data is included.

Use Export XML to save edits and Import XML to continue on another device. Data is kept in the browser session and is not synchronized or uploaded by this page. Download SIwave_Stackup_Studio.html for offline use. Reloading without exporting loses unsaved changes.

XML output follows the publicly documented Ansys Stackup namespace, nested material Double values, Layers LengthUnit, and FillMaterial. The importer also reads the tool's legacy Value-attribute format. It cancels unsupported layer types or extra advanced layer settings instead of dropping them. Colors and role metadata are kept in an XML comment for this editor; their application in SIwave is not guaranteed. Actual import in your installed SIwave version still needs verification.

Primary references:
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v252/en/Subsystems/SIwave/Content/EditingLayerProperties.htm
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v242/en/Subsystems/SIwave/Content/TNLayoutandODBControlFile.htm
- https://github.com/ansys/pyedb/blob/main/tests/example_models/TEDB/ansys_pcb_stackup.xml

No source from unrelated projects, photographs, account credentials, or local task records belongs in this deployment directory.
