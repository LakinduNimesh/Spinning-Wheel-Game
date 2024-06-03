# Spinning Wheel Game

## Overview

The Spinning Wheel Game is a web-based interactive game where users can spin a wheel and receive a random result. The wheel is implemented using HTML5, CSS, and JavaScript, with Chart.js used to create the pie chart for the wheel. The project also incorporates a spinning animation and a user-friendly interface.


![image](https://github.com/LakinduNimesh/Spinning-Wheel-Game/assets/149768006/2181c1ce-0ed9-4335-8641-3cbb76ad7832)


## Features

- **Interactive Wheel**: A spinning wheel that provides a random value on each spin.
- **Responsive Design**: The game is designed to be responsive and works well on both desktop and mobile devices.
- **Animation**: Smooth spinning animation using JavaScript.
- **User Interface**: Clean and simple UI with a spin button and a display area for the result.



## Getting Started

### Prerequisites

To run this project locally, you need a modern web browser that supports HTML5 and JavaScript.

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/LakinduNimesh/Spinning-Wheel-Game.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Spinning-Wheel-Game
   ```

### Running the Game

1. Open the `index.html` file in your preferred web browser.

## Project Structure

- `index.html`: The main HTML file that contains the structure of the web page.
- `style.css`: The CSS file that styles the web page.
- `script.js`: The JavaScript file that contains the logic for the spinning wheel.
- `README.md`: This file.

## Code Explanation

### HTML

The HTML file sets up the basic structure of the web page, including the canvas for the wheel, the spin button, and an SVG arrow indicator.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Meta tags and links to external resources -->
</head>
<body>
  <div class="wrapper">
    <h1 align="center">Spinning Wheel</h1>
    <div class="container">
      <canvas id="wheel"></canvas>
      <button id="spin-btn">Spin</button>
      <svg id="Layer_1" data-name="Layer 1" width="65" height="65" viewBox="0 0 65 65" xmlns="http://www.w3.org/2000/svg">
        <!-- SVG content -->
      </svg>
    </div>
    <div id="final-value">
      <p>Click on spin button to start</p>
    </div>
  </div>
  <!-- External JS scripts -->
</body>
</html>
```

### CSS

The CSS file styles the page, ensuring a visually appealing and responsive design.

```css
/* Basic styling for the web page */
body {
  /* Background and layout settings */
}
.wrapper {
  /* Styling for the wrapper */
}
#spin-btn {
  /* Styling for the spin button */
}
/* Additional styles */
```

### JavaScript

The JavaScript file handles the logic for the spinning wheel, including the creation of the pie chart, the spinning animation, and displaying the result.

```javascript
const wheel = document.getElementById("wheel"),
  spinBtn = document.getElementById("spin-btn"),
  finalValue = document.getElementById("final-value");

// Configuration for the wheel
const rotationValues = [
  { minDegree: 0, maxDegree: 30, value: 2 },
  { minDegree: 31, maxDegree: 90, value: 1 },
  // Additional values
];
const data = [16, 16, 16, 16, 16, 16];
const pieColors = [
  "#924210dc",
  "#d49c5ce2",
  // Additional colors
];

// Create the wheel using Chart.js
let myChart = new Chart(wheel, {
  // Chart configuration
});

// Function to generate the result value
const valueGenerator = (angleValue) => {
  // Logic to determine the result value
};

// Event listener for the spin button
spinBtn.addEventListener("click", () => {
  // Logic to handle the spinning animation and display the result
});
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Thanks to the developers of [Chart.js](https://www.chartjs.org/) for the awesome chart library.
- Background image by [Pexels](https://images.pexels.com/photos/10524983/pexels-photo-10524983.jpeg).

---
