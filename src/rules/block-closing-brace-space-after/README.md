# block-closing-brace-space-after

Require or disallow a space after the closing brace of blocks.

```css
    a { color: pink; }
/**                  ↑  
 * The space after this brace */
```

## Options

`string`: `"always"|"never"`

### `"always"`

There *must always* be a single space after the closing brace.

The following patterns are considered warnings:

```css
a { color: pink; }b { color: red; }
```

The following patterns are *not* considered warnings:

```css
a { color: pink; } b { color: red; }
```

### `"never"`

There *must never* be whitespace after the closing brace.

The following patterns are considered warnings:

```css
a { color: pink; } b { color: red; }
```

The following patterns are *not* considered warnings:

```css
a { color: pink; }b { color: red; }
```