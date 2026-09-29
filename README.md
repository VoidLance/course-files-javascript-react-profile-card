# React Profile Card

A small React application that presents a team directory as a responsive collection of profile cards. Each card displays a profile image, name, role, biography, and skills.

## Why use this project?

- Provides a simple, reusable `ProfileCard` component.
- Demonstrates rendering a collection of data with React props and `.map()`.
- Includes responsive card and gallery styling.
- Shows a fallback message when a profile has no skills.
- Uses Create React App with React Testing Library for a familiar development workflow.

## Getting started

### Prerequisites

- Node.js and npm
- A modern web browser

### Installation

Clone the repository, move into the project directory, and install the dependencies:

```bash
git clone https://github.com/VoidLance/course-files-javascript-react-profile-card.git
cd course-files-javascript-react-profile-card
npm ci
```

### Start the development server

```bash
npm start
```

Open <http://localhost:3000> in your browser. The page reloads automatically when source files change.

### Create a production build

```bash
npm run build
```

The optimized output is written to the `build` directory.

## Usage

Profile data is defined in `src/App.js` and passed to `ProfileCard` as props:

```jsx
<ProfileCard
  name="Alex Morgan"
  title="Frontend Developer"
  imageUrl="https://example.com/alex.jpg"
  bio="Builds accessible and engaging interfaces."
  skills={["JavaScript", "React", "CSS"]}
/>
```

To add a team member, add an object with the same fields to the `profiles` array in `src/App.js`. The `skills` prop accepts an array of strings; an empty or missing array displays “No skills listed.”

## Available scripts

| Command | Description |
| --- | --- |
| `npm start` | Runs the development server. |
| `npm test` | Runs the test suite in interactive watch mode. |
| `npm run build` | Creates an optimized production build in `build/`. |
| `npm run eject` | Ejects Create React App configuration. This is irreversible and usually unnecessary. |

## Project structure

```text
src/
├── App.js          # Profile data and page layout
├── ProfileCard.js  # Reusable profile card component
├── App.css         # Card and page styles
└── App.test.js     # Component tests
```

## Getting help

For React and Create React App usage, see the [React documentation](https://react.dev/) and [Create React App documentation](https://create-react-app.dev/docs/getting-started/).

If you find a bug or have a question about this project, [open an issue](https://github.com/VoidLance/course-files-javascript-react-profile-card/issues) with steps to reproduce the problem and relevant browser or Node.js details.

## Contributing

The project is maintained by [VoidLance](https://github.com/VoidLance) and its contributors. Contributions are welcome:

1. Fork the repository and create a focused branch.
2. Install dependencies with `npm ci`.
3. Make your changes and run `npm test` and `npm run build`.
4. Open a pull request describing the change and its testing.

Please keep changes focused, preserve the existing component API where possible, and update this README when setup or usage changes.

## License

No license file is currently included. Add or consult the repository's licensing terms before redistributing the project.
