# Car reviewer
# 3D City and Car Viewer

This project is an interactive 3D viewer built with Three.js, designed to visualize a city environment and multiple car models. Users can explore the scene, interact with cars, and control their movement through keyboard inputs.

## Features

### Scene and Lighting
- A 3D scene with realistic ambient and directional lighting.
- Includes a city model for a comprehensive environment.

### Camera and Controls
- **OrbitControls** for rotating, panning, and zooming the camera interactively.
- Smooth camera transitions to focus on selected objects.

### Model Loading
- Loads multiple `.gltf` car models (Lamborghini and Mercedes-Benz).
- A city model serves as the backdrop for exploring the environment.

### Interactivity
- **Mouse Click Interaction**: Click on cars to smoothly zoom and focus on them.
- **Keyboard Controls**: Move selected cars with arrow keys:
  - **Arrow Up**: Move the car forward.
  - **Arrow Down**: Move the car backward.
  - **Arrow Left**: Rotate the car left.
  - **Arrow Right**: Rotate the car right.
- Camera dynamically follows the selected car during movement.

### Responsive Design
- Adjusts seamlessly to window resizing for consistent viewing across devices.

## Prerequisites

Ensure you have the following to run the project:

1. A web browser supporting WebGL.
2. A local server to host the files (e.g., VS Code Live Server, Python's `http.server`, etc.).

## Setup

1. Clone or download the repository.
2. Place the required model files in the following paths:
   - `./lamborghini_centenario_lp-770_interior_sdc/scene.gltf`
   - `./lamborghini_centenario_roadster_sdc/scene.gltf`
   - `./mersedes-benz_g63_amg/scene.gltf`
   - `./city_rtx/scene.gltf`
3. Open the `index.html` file in your browser using a local server.

## How It Works

### Interaction

- **Selecting Cars**:
  - Click on a car to highlight it and bring the camera into focus.
- **Moving Cars**:
  - Use the arrow keys to move and rotate the selected car.
  - The camera follows the car's position dynamically.

### Smooth Transitions
- Smooth zooming and focusing on cars when clicked.
- Interpolated camera and control target adjustments for a fluid experience.

### Rendering
- Continuous updates to the scene via the `animate()` function ensure smooth interactions and rendering.

## Dependencies

- [Three.js](https://threejs.org)
- [GLTFLoader](https://threejs.org/docs/#examples/en/loaders/GLTFLoader)
- [OrbitControls](https://threejs.org/docs/#examples/en/controls/OrbitControls)

## Future Enhancements

- Add more car models and animations.
- Implement collision detection for realistic interactions between cars and the environment.
- Allow users to upload their own 3D models for viewing.
- Introduce lighting effects for different times of day.
