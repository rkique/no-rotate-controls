# Pan Controls!

This is a modified version of trackball-controls.js for Three.js, where one-touch, left mouse, and right mouse all map to pan. Two touch, middle mouse, or the "S" key can still be used for zoom. This makes it the ideal controls for 2D displays utilizing Three.js for parallax.

Basic usage:

```
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

const renderer = new THREE.WebGLRenderer();
renderer.setSize( window.innerWidth, window.innerHeight );
document.body.appendChild( renderer.domElement );

var controls = new THREE.PanControls(camera, renderer.domElement);
```

Make sure that you have loaded `three.js` first.
