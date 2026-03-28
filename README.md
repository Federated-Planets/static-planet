# Static Planet Reference Implementation

This repository serves as the **official reference implementation** for a basic planetary landing site in the [Federated Planets](https://github.com/Federated-Planets/federated-planets) universe.

For detailed information on how the Federated Planets world works, including deterministic coordinate calculation and joining the federation, please refer to the [official specification](https://github.com/Federated-Planets/federated-planets).

## Reference Structure

To serve as a standard planet, this project includes:

- **`public/index.html`**: The source **Landing Site** of the planet.
- **`public/planet.css` & `public/map.js`**: Centralized styles and interactivity for the planet and its map.
- **`public/manifest.json`**: The metadata file for your planet.
- **`dist/`**: The generated output directory containing the synchronized site.
- **`scripts/update-map.js`**: The build script that parses the HTML links and generates deterministic coordinates.

## Development and Build

1.  **Customize your planet:** Edit `public/index.html` and `public/manifest.json`.
2.  **Update coordinates:** Every time you add or change links in the Warp Ring, run:
    ```bash
    npm install  # First time only
    npm run build
    ```
3.  **Local Preview:** Use `npm start` to serve the `dist/` folder.
