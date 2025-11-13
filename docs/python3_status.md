# Python 3 Status

StaSh has completed its migration to Python 3 and now targets the Python 3
runtime that ships with Pythonista 3 as well as standard desktop CPython 3.
The legacy Pythonista 2 (Python 2) runtime is no longer supported.

## What this means

- New code, documentation, and examples should assume Python 3 semantics.
- When porting StaSh to another platform (see `docs/porting_guide.md`), make
  sure the UI and installer integrate with a Python 3 environment.
- Compatibility shims that reference `py2` (for example the
  `SITE_PACKAGES_FOLDER_6` constant used by `pip`) are retained only so StaSh
  can coexist with older installations. New contributions should not rely on
  Python 2 specific behavior.

Please open an issue if you discover commands or modules that still depend on
Python 2 so they can be updated.
