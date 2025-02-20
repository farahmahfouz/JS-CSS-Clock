# JavaScript + CSS Clock

## Overview
This project is a simple, functional analog clock built using HTML, CSS, and JavaScript. The clock updates every second, displaying the current time with animated hands for hours, minutes, and seconds.

## Technologies Used
- **HTML**: Structure of the clock.
- **CSS**: Styling and positioning of the clock hands.
- **JavaScript**: Updates the clock hands dynamically using the `setInterval` function.

## Features
- Real-time clock updates every second.
- Smooth transition of the clock hands.
- Aesthetic design using CSS.

## File Structure
```
|-- index.html       # Main HTML file
|-- style.css        # Styles for the clock
|-- script.js        # JavaScript logic for updating the clock
```

## How It Works
1. The clock consists of three hands: hour, minute, and second.
2. The `setDate` function fetches the current time using `new Date()`.
3. The function calculates the rotation angles for each hand:
   - **Seconds hand**: `(seconds / 60) * 360 + 90` degrees
   - **Minutes hand**: `(minutes / 60) * 360 + (seconds / 60) * 6 + 90` degrees
   - **Hour hand**: `(hours / 12) * 360 + (minutes / 60) * 30 + 90` degrees
4. These values are applied to the `transform: rotate()` property to rotate the hands.
5. The `setInterval` function ensures the clock updates every second.

## Deployment
The project is deployed on Vercel. You can view it live at:

**[Live Demo](https://js-css-clock-fawn.vercel.app/)**

## How to Run Locally
1. Clone the repository:
   ```sh
   git clone https://github.com/farahmahfouz/JS-CSS-Clock.git
   ```
2. Navigate to the project folder:
   ```sh
   cd js-css-clock
   ```
3. Open `index.html` in a browser.

## License
This project is open-source and available under the MIT License.

---
Feel free to update the Vercel link once deployed!

