# Getting Started with Dot App

This project was bootstrapped with [Vite](https://vitejs.dev/).

When component (face or document) is initiliazed, sam.wasm file will be fetched from http://localhost:3000/sam.wasm.
That's why sam.wasm file need to be placed in root of public folder.

## License

In order to use these components integrated in the samples you will need a license agreement.

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://vitejs.dev/guide/build.html) for more information.

### `yarn copy-wasm`

For detection to work `wasm` folder with web assembly files in it has to be present in `public` folder.
This script copies wasm folder from node modules into public folder. 

```
yarn copy-wasm
```

or do it manually:

Copy `wasm` folder from `node_modules/@innovatrics/dot-document-auto-capture` or other auto-capture package to `reactjs-components-integration/public` folder.

## Docker 

In the main project directory exists a `Dockerfile` and `docker-compose.yml`. It is required that you have DockerDesktop running in your local-dev environment.

You can run the following Docker commands in the root of the folder:

### `docker build -t my-dot-app .`

This will build the docker image `my-dot-app`.

### `docker run -p 5173:5173 my-dot-app`

This will run the `my-dot-app` image on the [http://localhost:5173](http://localhost:5173).

## Learn More

You can learn more in the [Vite documentation](https://vitejs.dev/guide/).

To learn React, check out the [React documentation](https://reactjs.org/).
