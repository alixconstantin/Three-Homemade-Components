# Three-Homemade-Components

##  Reusable threeJS components with Vite

## 🍥 Build a vite ThreeJS component 🍥


1. Start by create a basic vite project 
```sh
npm create vite@latest
```
- select name project
- select Vanilla or your framework
- select if you want to writte it with JavaScript or TypeScript
- then : 
```sh
npm install 
npm run dev 
```

2. Install ThreeJS  
- install ThreeJS :
```sh
npm install three
```
3. Install a debugger ( optional )
- install Debug UI : 
```sh
npm install dat.gui
```
- then :
```sh
import * as dat from 'dat.gui'
const gui = new dat.GUI()
```
- use exemple : 
```sh
gui.add(material, "metalness").min(0).max(1).step(0.0001);
gui.add(material, "roughness").min(0).max(1).step(0.0001);
```
4. Install Orbit control for a global mouse control on 3D Scene ( optional ) :
- import it from node_modules : 
```sh
import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls.js'
```
- For it to work, you must provide the camera and the element in the page that will handle the mouse events as parameters:
```sh
const controls = new OrbitControls(camera, canvas)
```
- You can smooth the animation by adding some kind of acceleration and friction formulas :
```sh
controls.enableDamping = true
// dont forget to add it in your framerate control 
const tick = () =>
{
    // ...

    // Update controls
    controls.update()

    // ...
}

```



##  🍥 Three-Basic-Quick-Start component 🍥 

Here is the basic quick start components for fastly start a 3D Scene with all the basics necesarry component, feel free to remove or modify any parts for your own starter. 

- Download the component from Github
- on Terminal at root project for install native Vite dependencies : 
```sh
 cd project
 npm install
```
- for run the component : 
```sh
npm run dev
```

