# Pan Controls!

This is a modified version of [trackball-controls.js](https://github.com/mrdoob/three.js/blob/master/examples/js/controls/TrackballControls.js) for Three.js that removes the rotate functionality. See the official [Three.js docs for trackball-controls](https://threejs.org/docs/#examples/en/controls/TrackballControls) as well.
It is optimized for both desktop and mobile, with one-touch, left mouse, and right mouse all mapping to pan. Two touch, middle mouse, or the "S" key can still be used for zooming.

This makes it the ideal controls for 2D displays utilizing Three.js for parallax.

![Demo](https://raw.githubusercontent.com/rkique/threejs-pan-controls/master/pan-controls-demo.gif)

Basic usage:

Make sure you have set up your Three.js scene.

```
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

const renderer = new THREE.WebGLRenderer();
renderer.setSize( window.innerWidth, window.innerHeight );
document.body.appendChild( renderer.domElement );
```

And then add the THREE.PanControls object.

```
var controls = new THREE.PanControls(camera, renderer.domElement);
```
