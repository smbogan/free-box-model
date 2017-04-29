
## Box Model

### Box Anchor Points:

For a box named `a`:

1. Edges
  1. Left: `|a`
  1. Right: `a|`
  1. Top: `a^` OR `^a`
  1. Bottom: `a_` OR `_a`
1. Corners:
  1. Lower Left: `.a`
  1. Upper Left: `'a`
  1. Upper Right: `a'`
  1. Lower Right: `a.`
  
### Constraints:

To ensure that the lower left corner of `a` is in the same position as upper right corner of b, use:

`.a = b'`

