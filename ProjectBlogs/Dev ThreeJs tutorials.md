# ThreeJs tutorials

## Creating a scene

### First of All
To actually be able to display anything with three.js, we need three things: scene, camera and renderer, so that we can render the scene with camera.

#### main.js example
```javascript
import * as THREE from 'three';

const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

const renderer = new THREE.WebGLRenderer();
renderer.setSize( window.innerWidth, window.innerHeight );
document.body.appendChild( renderer.domElement );
```

### Camera
There are a few different cameras in three.js. For now, let's use a PerspectiveCamera.