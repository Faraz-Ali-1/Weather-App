# WeatherLy

WeatherLy is a dynamic, real-time weather forecasting application. By integrating with the OpenWeatherMap API, it provides users with up-to-the-minute weather data for any city globally, featuring a clean, responsive interface and localized data formatting.

---

![img](https://github.com/Faraz-Ali-1/Weather-App/blob/bf83b9396889956dd50121dcf9dfdc0150a81cec/screenshots/weather%201.jpg)

---

## Live Demo

https://faraz-ali-1.github.io/Weather-App/

---

## Technical Features

### Live API Integration
Implemented high-performance asynchronous data fetching using the **Fetch API** and **Async/Await**. The app communicates with the OpenWeatherMap REST API to retrieve temperature, wind speed, humidity, and atmospheric pressure.

### Advanced Localization
Utilized the **JavaScript Intl API** (`Intl.DisplayNames` and `Intl.DateTimeFormat`) to automatically convert country codes into full names and format unix timestamps into human-readable local dates and times.

### Dynamic UI States
Developed logic to transform raw API data into visual elements. This includes dynamically updating weather icons, calculating Celsius from Kelvin, and applying custom CSS filters (like drop-shadows) based on specific weather conditions (e.g., cloudy states).

### Responsive Grid Layout
Designed a mobile-first "Attributes" grid using CSS Flexbox. The UI intelligently shifts from a multi-column layout on desktops to a centered, high-readability stack on smaller mobile screens.

---

## Technical Challenges

### Data Parsing & Unit Conversion
The OpenWeatherMap API returns temperatures in Kelvin. I implemented a conversion formula ($$Celsius = Kelvin - 273.15$$) and used `.toFixed()` to ensure the UI remains clean and user-friendly without unnecessary decimal points.

### Error Handling & User Feedback
To prevent the app from breaking on invalid inputs, I integrated a `try...catch` block around the API request. If a user searches for a city that doesn't exist, the app provides immediate feedback via an alert rather than failing silently.

---

![](https://github.com/Faraz-Ali-1/Weather-App/blob/bf83b9396889956dd50121dcf9dfdc0150a81cec/screenshots/weather%202.jpg)

---

## Tech Stack

* **Logic:** JavaScript (ES6+), Async/Await
* **API:** OpenWeatherMap REST API
* **Formatting:** JavaScript Intl API
* **Icons:** FontAwesome, IonIcons
* **Styling:** CSS3 (Flexbox, Grid, Custom Variables)

---

## Installation

1. Clone the repository.
2. Open `index.html` in your browser.
3. Enter any city name in the search bar to see live weather data.

---

## License

This project is licensed under the MIT License.
