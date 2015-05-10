# torus-mesh

[![stable](http://badges.github.io/stability-badges/dist/stable.svg)](http://github.com/badges/stability-badges)

Generates an indexed 3D torus mesh.

```js
var torus = require('torus-mesh')
var mesh = torus()

console.log(mesh)
=> { positions, cells, normals, uvs }
```

It returns a simplicial complex, but also includes `normals` and `uvs` for lighting and texturing.

## Usage

[![NPM](https://nodei.co/npm/torus-mesh.png)](https://nodei.co/npm/torus-mesh/)

#### `mesh = torus([opt])`

Creates a new torus with options:

- `majorRadius` the radius of the major ring `R`, default 1.0
- `minorRadius` the radius of the minor ring `r`, default 0.25
- `majorSegments` the number of segments for the major ring, default 32
- `minorSegments` the number of segments for the minor ring, defualt 64
- `arc` the arc to draw, default `Math.PI * 2` (full circle)

## License

MIT. See [LICENSE.md](http://github.com/stackgl/torus-mesh/blob/master/LICENSE.md) for details.
