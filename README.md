# 🌍 TypeScript Geolocation Utils

![GitHub release](https://img.shields.io/github/release/Rdg-jmz/typescript-geolocation-utils.svg) ![npm](https://img.shields.io/npm/v/typescript-geolocation-utils.svg) ![GitHub issues](https://img.shields.io/github/issues/Rdg-jmz/typescript-geolocation-utils.svg)

Welcome to **TypeScript Geolocation Utils**! This lightweight utility helps you easily fetch a user's geolocation using the browser's native Geolocation API. With a simple, Promise-based design, it’s perfect for modern frontend applications. 

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Contributing](#contributing)
- [License](#license)
- [Release Notes](#release-notes)

## Features

- **Lightweight**: Minimal footprint for quick integration.
- **Promise-based**: Enjoy a clean and modern asynchronous approach.
- **Browser Compatibility**: Works seamlessly across all modern browsers.
- **TypeScript Support**: Fully typed for better development experience.
- **Easy to Use**: Simple API that anyone can understand.

## Installation

To install **TypeScript Geolocation Utils**, you can use npm or yarn. Run the following command in your terminal:

```bash
npm install typescript-geolocation-utils
```

or

```bash
yarn add typescript-geolocation-utils
```

## Usage

To get started, simply import the utility in your TypeScript or JavaScript file:

```typescript
import { getGeolocation } from 'typescript-geolocation-utils';

getGeolocation()
  .then((location) => {
    console.log('User Location:', location);
  })
  .catch((error) => {
    console.error('Error fetching location:', error);
  });
```

This code will log the user's latitude, longitude, and accuracy to the console. 

## API

### `getGeolocation()`

This function fetches the user's current geolocation. It returns a Promise that resolves to an object containing the following properties:

- **latitude**: The user's latitude.
- **longitude**: The user's longitude.
- **accuracy**: The accuracy of the location in meters.

#### Example

```typescript
const fetchLocation = async () => {
  try {
    const location = await getGeolocation();
    console.log(`Latitude: ${location.latitude}, Longitude: ${location.longitude}`);
  } catch (error) {
    console.error('Failed to fetch location:', error);
  }
};

fetchLocation();
```

## Contributing

We welcome contributions! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

Your contributions help improve this utility for everyone.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Release Notes

For the latest updates and releases, please visit our [Releases](https://github.com/Rdg-jmz/typescript-geolocation-utils/releases) section. Here, you can download the latest version and execute it in your projects.

---

Thank you for checking out **TypeScript Geolocation Utils**! We hope this utility makes it easier for you to work with geolocation in your applications. If you have any questions or suggestions, feel free to reach out or open an issue. Happy coding! 

For more information on releases, visit [Releases](https://github.com/Rdg-jmz/typescript-geolocation-utils/releases).