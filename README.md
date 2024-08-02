# Text Editor PWA

## Description

Text Editor PWA is a Progressive Web Application (PWA) that allows users to create, edit, and save text documents. The application leverages modern web technologies to offer offline capabilities, making it accessible even without an internet connection.

## Table of Contents

- [Description](#description)
- [Table of Contents](#table-of-contents)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Deployment](#deployment)
- [License](#license)
- [Contributing](#contributing)

## Features

- **Offline Access:** Users can access the text editor even without an internet connection.
- **IndexedDB Integration:** Saves and retrieves text data from the browser's IndexedDB.
- **Service Worker:** Uses a service worker to cache assets and provide offline functionality.
- **PWA Manifest:** Configures the PWA manifest for installability on mobile and desktop devices.
- **Webpack Bundling:** Uses Webpack to bundle JavaScript, CSS, and other assets.

## Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/aleroas/text-editor-pwa.git
    cd text-editor-pwa
    ```

2. **Install Dependencies:**

    Make sure you have Node.js and npm installed. Then, run:

    ```bash
    npm install
    ```

3. **Build the Application:**

    ```bash
    npm run build
    ```

4. **Start the Development Server:**

    ```bash
    npm start
    ```

## Usage

1. Open your browser and navigate to `http://localhost:8080` (or the port specified by Webpack).
2. Start typing in the text area. Your text is automatically saved to IndexedDB.
3. To install the PWA, use the "Add to Home Screen" prompt on mobile or the install button on supported browsers.

## Technologies Used

- **JavaScript (ES6+):** Modern JavaScript syntax and features.
- **Webpack:** Module bundler for JavaScript, CSS, and other assets.
- **Babel:** JavaScript compiler to ensure compatibility with older browsers.
- **IndexedDB:** Browser storage API for saving and retrieving text data.
- **Workbox:** Service worker library to cache assets and provide offline functionality.
- **HTML & CSS:** Basic structure and styling for the application.

## Deployment

The application can be deployed to various platforms. Here's a general guide for deploying to Render:

1. **Create a new web service on Render:**

    Go to [Render](https://render.com/) and create a new web service. Connect it to your GitHub repository.

2. **Configure Build and Start Commands:**

    In the build settings on Render, set the following:

    - **Build Command:**

        ```bash
        npm install && npm run build
        ```

    - **Start Command:**

        ```bash
        npm start
        ```

3. **Deploy:**

    Render will automatically build and deploy your application. Once deployed, you can access it via the provided URL.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
