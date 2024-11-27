# Stopwatch App: React
Welcome to the Stopwatch App, a simple React-based application that functions as a precise stopwatch. The app features start, stop, and reset functionality and provides time in minutes, seconds, and milliseconds.

You can access the deployed app here: [Stopwatch App](https://sudhasai783.github.io/Stop-watch-React-App/)

## Features
- **Start Timer**: Begin tracking elapsed time with a single click.
- **Stop Timer**: Pause the timer while preserving the elapsed time.
- **Reset Timer**: Reset the elapsed time back to zero.
- **Real-Time Updates**: Timer updates every 10 milliseconds.
- **Formatted Time Display**: Time is displayed in `MM:SS:MS` format with leading zero padding for consistency.

## Tech Stack
- **Frontend**: React
- **State Management**: React's `useState` Hook
- **Lifecycle Management**: React's `useEffect` Hook
- **References**: React's `useRef` Hook
- **Styling**: CSS (basic styles for layout)
- **Deployment**: GitHub Pages

## Access the App
[Stopwatch App](https://sudhasai783.github.io/Stop-watch-React-App/)

## How it Works
This app uses React hooks to manage the state, lifecycle, and references required for the stopwatch functionality.

- **`useState`**: Maintains the current elapsed time (`elapsedTime`) and whether the stopwatch is running (`isRunning`).
- **`useEffect`**: Sets up an interval when the stopwatch is running and clears it when stopped or the component is unmounted.
- **`useRef`**: Stores references for the interval ID and start time to avoid reinitializing them on re-renders.

### Time Formatting
The app includes a `formatTime` function that:
1. Converts the total elapsed time (in milliseconds) into hours, minutes, seconds, and milliseconds.
2. Pads single-digit values with leading zeros for consistency.
3. Displays the formatted time in `MM:SS:MS` format.

