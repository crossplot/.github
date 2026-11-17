<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="crossplot-wordmark-dark.svg" />
    <img src="crossplot-wordmark-light.svg" alt="crossplot" width="320" />
  </picture>
</p>

<p align="center"><b>Coordinated, cross-filtered charts for TypeScript.</b><br />A modern take on dc.js.</p>

Brush one chart and every linked chart re-aggregates. crossplot owns the hard parts, a fast
cross-filter engine and a shared filter store, and hands drawing to pluggable renderers, starting
with [Observable Plot](https://observablehq.com/plot/).

- **Zero-dependency core.** `@crossplot/core` is headless and has no runtime dependencies.
- **Off the main thread.** The engine runs in a Web Worker and updates only the rows a brush touches.
- **Declarative.** A chart is a plain object: a dimension, an aggregate and a view.
- **Opt-in everything else.** Renderers and framework wrappers are separate packages.

| Package | |
| --- | --- |
| `@crossplot/core` | Engine, filter store, dashboard model |
| `@crossplot/plot` | Observable Plot renderer |

crossplot is in early development and not on npm yet. Follow along in
[crossplot/crossplot](https://github.com/crossplot/crossplot).
