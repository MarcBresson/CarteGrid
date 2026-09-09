<p align="center">
  <img src="https://media.githubusercontent.com/media/MarcBresson/cartegrid/refs/heads/main/Resources/logos/cartegrid-logo.png" alt="CarteGrid logo" width="200">
</p>

# CarteGrid

**CarteGrid** is a FreeCAD addon for batch-exporting parametrized variants of a model. Define a
parameter grid over an `App::VarSet`'s properties, and it expands into named **variations**: for
each one, CarteGrid applies the values, recomputes the document, and exports your chosen objects
to whatever format FreeCAD itself can produce (STEP, STL, IGES, OBJ, 3MF, and more) — nothing
hardcoded to a single format.

Need a bracket in 4 lengths, 2 heights, and 2 widths, exported to both STEP and STL? CarteGrid defines
that sweep once and exports all 32 resulting files, correctly named, without touching the model
by hand.

[![Docs](https://github.com/MarcBresson/cartegrid/actions/workflows/docs.yml/badge.svg)](https://github.com/MarcBresson/cartegrid/actions/workflows/docs.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

**[Read the full documentation](https://cartegrid.readthedocs.io)**: installation, a
quickstart, a full tour of the dialog, and detailed guides.

![CarteGrid dialog in FreeCAD](https://media.githubusercontent.com/media/MarcBresson/cartegrid/refs/heads/main/Resources/Media/main-dialog.png)

## Why you'll like it

- A [scikit-learn `ParameterGrid`](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.ParameterGrid.html)-style
  parameter grid, with `Fixed`, `List`, `LinSpace`, and `Range` value kinds.
- Flexible naming templates, with duplicate-name protection before export runs.
- A tree-based object picker that hides Body-internal features by default, showing only
  finished, exportable parts.
- Per-format export preferences: a global preferred-formats list, with an optional per-item
  override.
- Your VarSet's values are always restored after export, whether it succeeds or fails partway
  through.
- A VarSet-to-CSV export, handy for generating parameter documentation alongside your files.
- Configuration is saved inside the document itself (no sidecar files), and a document can
  hold more than one configuration, one per body, for example.

## Getting started

Install via FreeCAD's **Tools ▸ Addon Manager** (search "CarteGrid"), then follow the
[quickstart](https://cartegrid.readthedocs.io/en/latest/quickstart.html) to run your
first export in a few minutes.

## Contributing

See the [contributing guide](https://cartegrid.readthedocs.io/en/latest/contributing.html)
for setting up a development install and running the test suite.

## License

[MIT](LICENSE)
