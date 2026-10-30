# SIwave Stackup Studio

Standalone HTML tool for PCB stackup editing. Open index.html in a browser or use the GitHub Pages website. No installation, server, account, or external page dependency is required. This is an independent helper, not an Ansys product.

v3.0 defaults to numbering conductor names L1,L2,... from top to bottom. Dielectric and solder-mask names remain unchanged and do not consume an L number. Naming follows count, insertion, deletion and ordering; all other layer properties stay intact. Editing a conductor name manually switches to custom mode; imported XML names are preserved unless validated editor metadata restores automatic mode. The checkbox can explicitly renumber current layers, with collision protection for nonconductor names. Naming mode is preserved in the editor XML comment and layer-count undo snapshot.

Copper-count changes still commit when input is finished (on change/blur), with Apply and Enter retained and an immediate16-copper quick selection. Reductions require confirmation and support undo. All detail rows expand in the page; preview uses an explicit expand/collapse button instead of an internal vertical scrollbar. Phone-width tables still scroll horizontally to keep columns readable.

The SIwave table column order, material-derived electrical values, selectable metal-layer dielectric fill, and local preview colors remain available. Basic editing and original generic presets remain intact; no company-specific stackup photo or data is included.

Use Export XML to save edits and Import XML to continue on another device. Data is kept in the browser session and is not synchronized or uploaded by this page. Download SIwave_Stackup_Studio.html for offline use. Reloading without exporting loses unsaved changes.

XML output follows the publicly documented Ansys Stackup namespace, nested material Double values, Layers LengthUnit, and FillMaterial. The importer also reads the tool's legacy Value-attribute format. It cancels unsupported layer types or extra advanced layer settings instead of dropping them. Colors and role metadata are kept in an XML comment for this editor; their application in SIwave is not guaranteed. Actual import in your installed SIwave version still needs verification.

Primary references:
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v252/en/Subsystems/SIwave/Content/EditingLayerProperties.htm
- https://ansyshelp.ansys.com/public/Views/Secured/Electronics/v242/en/Subsystems/SIwave/Content/TNLayoutandODBControlFile.htm
- https://github.com/ansys/pyedb/blob/main/tests/example_models/TEDB/ansys_pcb_stackup.xml

No source from unrelated projects, photographs, account credentials, or local task records belongs in this deployment directory.
