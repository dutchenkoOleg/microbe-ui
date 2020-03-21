# IE Support

`insertNavHome`

**By default `microbe-ui` do not support Internet Explorer.** 
The main reason: we use CSS Custom Properties which has no support in IE.

But we has implemented degradation methodology in our [Code generation](./code-generation.md). 

You can set `true` value for `$microbe-ie-fallback` variable. That disable usage of CSS Custom Properties and change them by our fallbacks.

_**Warning!** Degradation methodology will increase CSS code size (about twice)!_

_Example:_

```scss
@import "~microbe-ui/src/core";

// enable IE support
$microbe-ie-fallback: true;

// add "Module grid" and "Spacer" components
@import "~microbe-ui/src/components/module-grid";
@import "~microbe-ui/src/components/spacer";
```

`insertNavDivider=ie-support`
