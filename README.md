# SIwave Stackup Studio

Standalone HTML tool for PCB stackup editing. Open index.html in a browser or use the GitHub Pages website. No installation, server, account, or external page dependency is required. This is an independent helper, not an Ansys product.

v2.8 adds the photographed SIwave table column order, material-derived electrical values, selectable metal-layer dielectric fill, and local preview colors. Basic editing remains available. Original generic presets remain intact; no company-specific stackup photo or data is included.

Use Export XML to save edits and Import XML to continue on another device. Data is kept in the browser session and is not synchronized or uploaded by this page. Download SIwave_Stackup_Studio.html for offline use. Reloading without exporting loses unsaved changes.

XML output follows the publicly documented Ansys Stackup namespace, nested material Double values, Layers LengthUnit, and FillMaterial. The importer also reads the tool's legacy Value-attribute format. It cancels unsupported layer types or extra advanced layer settings instead of dropping them. Colors and role metadata are kept in an XML comment for this editor; their application in SIwave is not guaranteed. Actual import in your installed SIwave version still needs verification.

Primary references:
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v252/en/Subsystems/SIwave/Content/EditingLayerProperties.htm
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v242/en/Subsystems/SIwave/Content/TNLayoutandODBControlFile.htm
- https://github.com/ansys/pyedb/blob/main/tests/example_models/TEDB/ansys_pcb_stackup.xml

No source from unrelated projects, photographs, account credentials, or local task records belongs in this deployment directory.
