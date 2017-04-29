
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

To say that box `a` is inside of `b`:

`a < b`

To free a box of all constraints:

`!a`

To free an anchor point of all constraints:

`!a'`, for example frees all constraints on `a'`.

To free all constraints between two boxes:

`a != b`

To free all constraints between two anchor points:

`.a != b'`

To free all constraints between a box and a specific anchor point on another box:

`a != b`

#### Spacer Constraints

A spacer is used where a box is not needed later, but spacing is required:

`b < a; |a = |$, $| = |b, {a.width = .1*$.width + .9*b.width};`
