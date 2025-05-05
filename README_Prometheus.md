# Expo Netflix UI Clone: A Cross-Platform Mobile Streaming App Showcase

## Project Overview

A comprehensive mobile application that delivers a pixel-perfect clone of the Netflix user interface using Expo and React Native. This project provides a fully responsive, mobile-friendly streaming service UI that mimics the core experience of the Netflix application.

### Core Purpose
The application aims to demonstrate a high-fidelity recreation of the Netflix mobile interface, showcasing advanced mobile UI/UX design and React Native development techniques. It serves as both a learning resource and a technical showcase for mobile app developers.

### Key Features
- Pixel-perfect Netflix UI replication
- Multi-screen navigation mimicking the Netflix app
- Comprehensive home screen with content categories
- Detailed movie and TV show browsing experience
- Profile management functionality
- Search and content discovery interfaces
- Responsive design supporting multiple platforms

### Benefits
- Provides an open-source reference implementation for mobile streaming app interfaces
- Demonstrates best practices in React Native development
- Offers a practical example of complex mobile UI design and navigation
- Serves as a learning tool for developers interested in mobile app development
- Showcases integration of modern mobile development technologies

## Getting Started, Installation, and Setup

### Prerequisites

- Node.js v16.14.2 (recommended using [nvm](https://github.com/nvm-sh/nvm))
- Yarn or npm package manager
- Expo CLI

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/expo-netflix.git
   cd expo-netflix
   ```

2. Install dependencies:
   ```bash
   yarn install
   # or
   npm install
   ```

### Development Setup

#### Running the App

You can run the app on multiple platforms using the following commands:

- For iOS (requires macOS and Xcode):
  ```bash
  yarn ios
  # or
  npm run ios
  ```

- For Android:
  ```bash
  yarn android
  # or
  npm run android
  ```

- For Web:
  ```bash
  yarn web
  # or
  npm run web
  ```

#### Quick Start

To start the development server:
```bash
yarn dev
# or
npm run dev
```

This will launch the Expo development client, allowing you to run the app on a simulator, emulator, or scan the QR code with the Expo Go app on your mobile device.

### Build for Production

#### Web Build
To create a production web build:
```bash
yarn web-build
# or
npm run web-build
```

### Additional Development Tools

- Linting:
  ```bash
  yarn lint
  # or
  npm run lint
  ```

### Notes

- This project uses Expo, which simplifies React Native development and deployment
- Ensure you have the latest version of Expo CLI installed globally
- For the best development experience, use Visual Studio Code with recommended React Native and Expo extensions

## Supported Platforms

The application is cross-platform and supports:

- Android
- iOS
- Web

#### Platform Compatibility
- Developed using Expo, enabling seamless multi-platform deployment
- Native support for mobile platforms (Android and iOS)
- Web version available using React Native Web

#### Platform-Specific Considerations
- Compatible with mobile and web environments
- Optimized for portrait orientation
- Tablet support available for iOS devices

#### Device Requirements
- Requires a device or emulator running:
  - Android (minimum version not specified)
  - iOS (minimum version not specified)
  - Modern web browser

## Running the App

### Prerequisites

- Node.js (version specified in `.nvmrc`)
- Expo CLI
- Yarn or npm
- Xcode (for iOS) or Android Studio (for Android)

### Running on Simulators/Emulators

#### iOS
```bash
expo start --ios
```

#### Android
```bash
expo start --android
```

### Running on Web
```bash
expo start --web
```

### Running Directly
```bash
expo start
```

### Device Testing
For physical device testing, install the Expo Go app from the App Store or Google Play Store, then scan the QR code displayed in the terminal when you run `expo start`.

#### Notes
- Ensure all dependencies are installed before running (`yarn install` or `npm install`)
- A stable internet connection is recommended for Expo development

## Key Screens and Features

The app provides a comprehensive Netflix-like mobile experience with several key screens and interactive features:

### Main Navigation
The application features a bottom tab navigation with four primary screens:
- Home: Browse and discover content
- Search: Find specific movies and shows
- Downloads: Manage downloaded content
- More: Access additional settings and profile options

### Home Screen
- Displays various content categories and recommendations
- Features a scrollable interface with Netflix-style horizontal content rows
- Includes a prominent header with profile and navigation options
- Supports quick access to content details and playback

### Search Screen
- Comprehensive content search functionality
- Real-time search results with content suggestions
- Allows users to find movies, TV shows, and specific titles

### Downloads Screen
- Manage downloaded content for offline viewing
- Track and organize downloaded movies and shows
- View storage usage and downloaded items

### Profile and Settings
- Multiple profile management
- Add, edit, and switch between user profiles
- Customize app settings and preferences

### Additional Features
- Content preview and detailed information
- Ability to add content to "My List"
- Cast connectivity for streaming to external devices
- Dark theme consistent with Netflix design aesthetics

## Build and Deployment

### Build Configurations

The project uses Expo for cross-platform development and build management. Production builds can be created using the following methods:

#### Web Build
To create a production web build, use the command:
```bash
yarn web-build
```

#### Mobile Platform Builds
The project supports builds for Android, iOS, and web platforms. To generate production builds, you'll need to use Expo's build services:

- **iOS**: Use Expo's build service or Xcode for App Store distribution
- **Android**: Use Expo's build service or Android Studio for Google Play Store distribution

### Distribution Platforms

- **Expo**: Supports distribution through Expo's platform
- **Web**: Deployable to standard web hosting services
- **Mobile**: Compatible with App Store (iOS) and Play Store (Android)

### Deployment Considerations

- Ensure you have the latest Expo CLI installed
- Configure app credentials in `app.json`
- Update version numbers in both `package.json` and `app.json`
- Current version: 0.0.2
- Supported platforms: Android, iOS, Web

## Project Structure

The project follows a structured React Native directory layout designed for modularity and scalability:

### Source Code Directory (`src/`)
The `src/` directory contains the core application code, organized into several key subdirectories:

#### Components (`src/components/`)
Contains reusable React components that are used across different screens of the application:
- UI elements like `Header`, `TouchText`, `ShowScroller`
- Specialized components such as `PromotionBanner`, `Cast`

#### Constants (`src/constants/`)
Stores application-wide constants and utility functions:
- `colors.js`: Color palette for the app
- `fonts.js`: Font definitions
- `globalStyles.js`: Shared styling configurations
- `preloadFonts.js` and `preloadImages.js`: Asset preloading utilities

#### Icons (`src/icons/`)
SVG icon components for various UI elements:
- Navigation icons (`Home`, `Search`, `Downloads`)
- Action icons (`Play`, `Plus`, `Edit`)
- Directional icons (`ArrowLeft`, `ArrowRight`)

#### Mock Data (`src/mockdata/`)
Contains JSON and JavaScript files with placeholder data:
- `data.js`: General mock data
- `myList.json`: Sample user playlist data
- `previews.json`: Content preview information

#### Navigation (`src/navigation/`)
Defines the app's navigation structure:
- `RootStack.js`: Main navigation configuration
- Stack navigators for different sections (`StackHome`, `StackSearch`)
- `TabNavigation.js`: Bottom tab navigation

#### Screens (`src/screens/`)
Individual screen components for different app views:
- Main screens: `Home`, `Search`, `Downloads`, `More`
- Modal screens: `ModalAddProfile`, `ModalManageProfiles`
- Content screens: `Movies`, `TvShows`, `MyList`

### Root Directory Files
- `App.js`: Main application entry point
- `app.json`: Expo/React Native configuration
- `package.json`: Project dependencies and scripts
- Configuration files: `.eslintrc`, `babel.config.js`

### Additional Directories
- `src/assets/`: Image assets, including logos, content images, and user icons
- `web/`: Web-specific files like `_index.html`

The project is structured to separate concerns, making it easy to maintain and extend the Netflix-like mobile application.

## Technologies Used

### Mobile Framework
- [Expo](https://expo.dev/) - A framework and platform for universal React Native apps
- [React Native](https://reactnative.dev/) - Mobile application development framework

### Navigation
- [React Navigation](https://reactnavigation.org/)
  - Bottom Tabs Navigation
  - Native Stack Navigation

### UI and Styling
- [React Native SVG](https://github.com/react-native-svg/react-native-svg) - SVG rendering for React Native
- [React Native Gesture Handler](https://docs.swmansion.com/react-native-gesture-handler/) - Native touches and gestures
- [React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/) - Animations library

### Expo Services
- Expo Asset Management
- Expo Device Information
- Expo Font Loading
- Expo Splash Screen
- Expo Updates

### Development Tools
- [ESLint](https://eslint.org/) - JavaScript linting
- [Prettier](https://prettier.io/) - Code formatting
- Babel - JavaScript compiler

### Web Support
- [React Native Web](https://necolas.github.io/react-native-web/) - React Native components and APIs for web

### Additional Libraries
- [PropTypes](https://www.npmjs.com/package/prop-types) - Runtime type checking for React props
- [React Native WebView](https://github.com/react-native-webview/react-native-webview) - WebView component for React Native

## Additional Notes

### Performance and Optimization

The application is built using Expo and optimized for cross-platform performance, with specific considerations for mobile and web platforms. Key optimization strategies include:

- Leveraging Expo's built-in performance optimization tools
- Using React Native's efficient rendering mechanisms
- Implementing code-splitting and lazy loading where applicable

### Accessibility Considerations

The project includes SVG icons and uses React Native Safe Area Context to ensure consistent layout across different device types. Developers should continue to enhance accessibility by:

- Maintaining proper color contrast
- Implementing screen reader support
- Ensuring touch targets meet minimum size requirements

### Known Limitations

- The current version uses mock data for content display
- Some advanced Netflix features may not be fully replicated
- Performance may vary across different device types and screen sizes

### Environment and Compatibility

- Supports React Native 0.73.2
- Compatible with Expo SDK 50
- Tested on iOS, Android, and Web platforms

### Development Insights

- ESLint and Prettier are configured for code quality and consistency
- Uses modern React Native navigation patterns
- Modular component structure in the `src/` directory

## Contributing

We welcome contributions to the Netflix UI Clone project! Here are some guidelines to help you contribute effectively:

### Code Style and Linting

The project uses ESLint with Airbnb configuration and Prettier for code formatting. Before submitting a pull request:

- Run `yarn lint` to check for any linting errors
- Ensure your code follows the project's ESLint rules
- Use Prettier for automatic code formatting
- Recommended IDE integrations:
  - Atom: prettier-atom package
  - VSCode: Prettier extension

### Development Setup

1. Fork the repository
2. Clone your forked repository
3. Install dependencies: `yarn`
4. Run the project locally: `yarn dev`

### Contribution Process

1. Create a new branch for your feature or bugfix
2. Make your changes
3. Write or update tests if applicable
4. Ensure all tests pass
5. Submit a pull request with a clear description of your changes

### Key Contribution Areas

- Bug fixes
- Performance improvements
- New feature implementations
- Documentation updates
- UI/UX enhancements

### Testing

- The project uses Jest for testing
- Ensure new features or bug fixes include appropriate test coverage
- Run existing tests before submitting a pull request

### Reporting Issues

- Use GitHub Issues to report bugs or suggest features
- Provide a clear and detailed description
- Include steps to reproduce the issue
- Attach screenshots or error logs if possible

### Code of Conduct

- Be respectful and collaborative
- Follow the project's existing code style and conventions
- Help maintain a welcoming and inclusive community

Thank you for your contributions!

## License

This project is licensed under the MIT License. 

### License Details
- **Type**: MIT License
- **Copyright**: © 2019 Caleb Nance

The MIT License is a permissive free software license that allows users to do almost anything with the project's code with limited restrictions. 

### Key Permissions
- Commercial use
- Modification
- Distribution
- Private use

### Conditions
- Include the original license and copyright notice in any substantial portion of the software

For the full license text, please see the [LICENSE](LICENSE) file in the repository.