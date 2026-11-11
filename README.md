# Chrono | Digital Clock & Alarm

A modern, responsive **Digital Clock and Alarm web application** built with **HTML, CSS, and JavaScript**.

Chrono allows users to view real-time local time, switch between 12-hour and 24-hour formats, create multiple alarms, and save their alarm preferences directly in their browser.

## Features

- Live digital clock displaying hours, minutes, and seconds
- Current date and local timezone display
- 12-hour and 24-hour clock formats
- Create multiple alarms with custom labels
- One-time and repeating alarms
- Enable, disable, and delete alarms
- Audible alarm notifications
- Five-minute snooze and dismiss functionality
- Light and dark themes
- Local Storage support for saving alarms
- Responsive design for desktop, tablet, and mobile
- No backend or database required

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive design |
| JavaScript (ES Modules) | Clock and alarm functionality |
| Local Storage | Save alarms and preferences |
| Web Audio API | Alarm sounds |
| Node.js | Optional automated testing |

## Installation and Setup in VS Code

### Step 1: Download the Project

1. Click the green **Code** button on this GitHub repository.
2. Select **Download ZIP**.
3. Extract the downloaded ZIP file.
4. Open Visual Studio Code.
5. Select **File > Open Folder**.
6. Choose the extracted `digital-clock-alarm` folder.

### Step 2: Install Live Server

The application uses JavaScript modules, so it should be opened through a local web server.

1. Open the Extensions panel in VS Code.
2. Search for **Live Server** by Ritwick Dey.
3. Install the extension.

### Step 3: Run the Application

1. Open `index.html`.
2. Right-click anywhere inside the file.
3. Select **Open with Live Server**.
4. The application will open automatically in your browser.

The local address will typically be:

`http://127.0.0.1:5500`

### Alternative: Run with Python

If Python is installed, you can run a local server from the VS Code terminal:

```bash
python -m http.server 8000
```

Then open:

`http://localhost:8000`

On Windows, you can alternatively run:

```bash
py -m http.server 8000
```

## How to Use

### Digital Clock

1. Open the application.
2. The clock automatically displays your local time.
3. Switch between 12-hour and 24-hour formats.
4. Toggle between light and dark themes.

### Setting an Alarm

1. Click **New alarm**.
2. Select your preferred alarm time.
3. Enter an optional alarm label.
4. Choose the weekdays for a repeating alarm, if needed.
5. Click **Save alarm**.
6. Keep the browser tab open and your device awake.

### Managing Alarms

- Enable or disable existing alarms.
- Delete alarms you no longer need.
- Snooze ringing alarms for five minutes.
- Dismiss alarms when they ring.
- Save alarm preferences automatically using Local Storage.

## Project Structure

```text
digital-clock-alarm/
├── index.html
├── assets/
│   ├── app.js
│   ├── core.mjs
│   └── styles.css
├── tests/
│   └── core.test.mjs
├── .gitignore
├── LICENSE
└── README.md
```

### File Descriptions

- **index.html:** Main application interface.
- **assets/styles.css:** Styling, animations, and responsive layouts.
- **assets/app.js:** Clock display, alarm management, and user interactions.
- **assets/core.mjs:** Core alarm scheduling and time formatting logic.
- **tests/core.test.mjs:** Automated tests.
- **.gitignore:** Excludes unnecessary development files.
- **LICENSE:** MIT License information.

## Running Automated Tests

Install Node.js version 18 or newer to run the automated tests.

Open your VS Code terminal and execute:

```bash
node --test tests/core.test.mjs
```

The tests check time validation, stored data parsing, time formatting, repeat schedules, and alarm-triggering logic.

Node.js is only required for testing. It is not required to use the web application.

## Deployment Using GitHub Pages

This project can be hosted for free using GitHub Pages.

### Deployment Steps

1. Create a public repository named `digital-clock-alarm`.
2. Upload all project files and folders.
3. Ensure `index.html` is in the repository's root directory.
4. Open **Settings** in your GitHub repository.
5. Select **Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select the `main` branch.
8. Select the `/(root)` folder.
9. Click **Save**.

After deployment completes, GitHub Pages will provide your live website URL.

No API keys, database, or environment variables are required.

## Important Notes

- The browser tab must remain open for alarms to work reliably.
- Browsers may suspend inactive tabs, and alarms may not ring if the computer is asleep.
- Some browsers restrict audio playback until the user interacts with the page.
- Alarm settings are saved locally in the browser.
- Clearing browser storage may remove saved alarms.
- Snooze settings do not persist after refreshing the page.
- This project is intended as a browser-based alarm application, not a replacement for a dedicated alarm clock.
- Google Fonts require an internet connection. Fallback fonts are available when offline.

## Contributing

Contributions, improvements, and suggestions are welcome.

1. Fork this repository.
2. Create a new branch.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

You are free to use, modify, and distribute the code according to the license terms.
