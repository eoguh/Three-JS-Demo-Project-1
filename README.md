# Three.js Demo Project 1

A simple 3D graphics project built with [Three.js](https://threejs.org/).

This project demonstrates the creation and animation of a 3D cube using Three.js, featuring basic scene setup, camera positioning, materials, lighting, and continuous rotation.

## Features

- Interactive 3D cube rendering.
- Continuously rotating cube animation.
- Custom background and cube colors.
- Directional lighting for enhanced visual appearance.
- Real-time 3D rendering using WebGL.

## Technologies Used

- JavaScript (ES6+)
- Three.js
- WebGL
- HTML5
- Import Maps
- jsDelivr CDN

## Prerequisites

Before running this project, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (which includes npm).
- A modern web browser with WebGL support.
- Git (optional, for cloning the repository).

## Getting Started

Follow these steps to download and run the project locally.

### 1. Clone the Repository

Open your terminal and run:

```bash
git clone https://github.com/eoguh/Three-JS-Demo-Project-1.git
```

### 2. Navigate to the Project Directory

```bash
cd Three-JS-Demo-Project-1
```

### 3. Set Up the Project Files

The project files are organized as follows:

```text
Three-JS-Demo-Project-1/
│
├── index.html
├── main.js
├── package.json
└── package-lock.json
```

**File descriptions:**

- `index.html` – The main HTML entry point containing the Import Map and JavaScript module reference.
- `main.js` – Contains the Three.js scene, camera, cube geometry, materials, lighting, and animation logic.
- `package.json` – Contains project metadata and dependencies/scripts.
- `package-lock.json` – Records dependency versions for consistent installations.

### 4. Run the Project

Since this project uses JavaScript ES modules and Import Maps, it should be served through a local development server rather than opened directly in your browser.

You can use Vite to run the project.

If Vite is not already installed, install it:

```bash
npm install --save-dev vite
```

Add the following scripts to the `scripts` section of your `package.json`:

```json
"scripts": {
  "dev": "vite",
  "build": "vite",
  "preview": "vite preview"
}
```

Start the development server:

```bash
npm run dev
```

Vite will start a local development server and display a URL, usually:

```text
http://localhost:5173/
```

Open this URL in your web browser to view the animated 3D cube.

## How It Works

The application uses Three.js to create and render a basic 3D scene.

- **Scene:** Creates the 3D environment and sets its background color.
- **Camera:** Defines the perspective and viewing position.
- **Geometry:** Creates a cube using `BoxGeometry`.
- **Material:** Applies color and surface properties to the cube.
- **Lighting:** Uses a directional light to illuminate the scene.
- **Renderer:** Renders the 3D scene inside the browser.
- **Animation:** Continuously rotates the cube along the X and Y axes.

## Customization

Feel free to experiment with the `main.js` file:

- Change the cube's color.
- Adjust the cube's rotation speed.
- Modify the camera position and viewing angle.
- Experiment with different lighting configurations.
- Change the background color.
- Replace `BoxGeometry` with other Three.js geometries such as SphereGeometry, TorusGeometry, or DodecahedronGeometry.

## Troubleshooting

**1. Blank screen or nothing renders?**

- Make sure you are running the project through a local development server.
- Check your browser's developer console for errors.
- Ensure your browser supports WebGL.

**2. Three.js import errors?**

Check that your Import Map in `index.html` points to a valid Three.js CDN URL:

```html
<script type="importmap">
{
  "imports": {
    "three": "https://cdn.jsdelivr.net/npm/three@0.187.0/build/three.module.js",
    "three/addons/": "https://cdn.jsdelivr.net/npm/three@0.187.0/examples/jsm/"
  }
}
</script>
```

**3. CDN loading issues?**

Ensure you have an active internet connection because Three.js is loaded from jsDelivr.

## Contributing

Suggestions, improvements, and contributions are welcome!

Feel free to fork this repository, experiment with the code, and submit a pull request.

## License

This project is open-source and available for learning, experimentation, and personal use.

---

**Built with Three.js 🚀**