# no-rotate-controls

This is a modified version of trackball-controls.js for Three.js where one-touch, left mouse, and right mouse all map to pan. Two touch, middle mouse, or the "S" key can still be used for zoom. This makes it the ideal controls for 2D displays utilizing Three.js for parallax.

Usage:
`var controls = new THREE.PanControls(camera, renderer.domElement);`
Make sure that you have loaded `three.js` first.
