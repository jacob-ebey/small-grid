# small-grid

A small responsive grid framework.

## Installing

```
npm install small-grid
```

## How to use

```typescript
import 'small-grid/small-grid.css';
```

Create a grid and add columns:

```html
<div class="grid">
  <div class="col s12 m6 l8">1</div>
  <div class="col s12 m6 l4">2</div>
</div>
```

The above markup is am example of a grid with two columns that both show 100% (across all 12 columns) on small devices, 50/50 columns on medium devices and 8/4 on large devices. We can actually obmit the **s12** as columns will always default to 100% if
a size is not specified for the breakpoint.

Column options:
- s{1-12} Show as spanning 1-12 columns when width >= 320px
- m{1-12} Show as spanning 1-12 columns when width >= 641px
- l{1-12} Show as spanning 1-12 columns when width >= 1025px


## Responsive helpers

These classes can be used like so to go from a single column on mobile to two columns on anything large:

```css
<div class="grid"
  <div class="col m6">1</div>
  <div class="col m6 show-m">2</div>
</div>
```

Options:
- s{1-12} Show when width >= 320px
- m{1-12} Show when width >= 641px
- l{1-12} Show when width >= 1025px
