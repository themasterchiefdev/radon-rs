# Compatibility baseline

Radon Rust analyzes **Python source**. Rust is its implementation language.

The source inventory is pinned to [`rubik/radon` commit `54b88e5878b2724bf4d77f97349588b811abdff2`](https://github.com/rubik/radon/tree/54b88e5878b2724bf4d77f97349588b811abdff2), identified as Radon 6.0.1 in the supplied inventory reviewed on 2026-08-19. Each row in [features.csv](features.csv) retains its upstream evidence link. “Not started” refers to the Rust port.

The initial target is native command-line behavior and the four metric families. The supported Python syntax range, Python API compatibility, module invocation, Flake8, and legacy Code Climate runtime selection still require decisions. A listed source capability is not a promise that it will ship unchanged.

Two source/documentation discrepancies need executable examples:

- RAD-039: `with` and `async with` contribute no complexity in the pinned visitor; explanatory text differs.
- RAD-076: the pinned Maintainability Index code uses logical lines and a comment factor of 2.46; the inventory records different documentation.

RAD-066, RAD-075, and RAD-084 describe upstream unsupported exports. Preserve them as negative compatibility cases unless a documented scope decision changes them.

Compare implementations on shared inputs with pinned upstream results. Include normal inputs, empty inputs, syntax errors, nested and asynchronous constructs, and metric boundaries. Define numeric tolerances where needed. Do not infer execution from a test reference: the supplied inventory reports that its pytest and CLI verification did not run.

No compatibility or performance suite has run for this port yet.
