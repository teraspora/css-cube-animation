# Cube animation

This is a basic animation of a cube, which I made in order to learn about CSS transitions, transforms and animations.

I create 6 faces then transform them by translation and rotation into their correct positions:  the front needs no rotation, the back 180° about either the X- or Y- axis, while the top, bottom, left and right need 90° rotations either way about the X- or Y-axis.   The coordinate system rotates with the element, so it's always the Z-axis that points out of each face even when it's been rotated, thus, in order that we don't just have three orthogonal planes intersecting at the origin, we then need to translate each face outwards (i.e along the +ve Z-axis by half the width.

The properties

```css
display: flex;
align-items: center;
justify-content: center;
```
of the enclosing div seem to be critical in getting the thing positioned correctly.   I had great trouble until I discovered this!

The animation just gradually zooms in and rotates about each axis in turn.

Many thanks to the authors of all the many tutorials and guides to CSS transforms and animations that have taught me what I have learned so far.

## To do:

- Factor out widths and heights into custom properties (a.k.a.CSS variables).

- Learn Sass properly so I can do the keyframes etc. in a loop.

- Add some Javascript so I can change the images when the cube is at its smallest.

- Try translating along the Z-axis instead of scaling, and experiment with the perspective and perspective-origin properties in conjunction with this.
