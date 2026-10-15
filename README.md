# MoodMode

MoodMode is a customizable productivity dashboard that helps you organize your day around routines, focus presets, and short brain breaks.

## Features

- **Customizable spaces:** Organize presets by group or area of your life.
- **Focus presets:** Create presets with an emoji, description, priority, start time, timer, active days, accent color, and app or website links.
- **Daily routine:** View your routine and see what is scheduled next.
- **Focus timer:** Start, pause, extend, or stop a timed session.
- **Reminders:** Enable browser notifications for scheduled routine items.
- **Appearance settings:** Customize colors, backgrounds, fonts, spacing, card styles, and layout.
- **Productive breaks:** Play small activities such as Focus Typer, Math Sprint, Word Forge, Memory Matrix, and Logic Quiz.
- **Local progress tracking:** Saves settings, presets, and game scores in your browser's local storage.
- **Import and export:** Export a space's settings and presets or import a saved JSON file.
- **Optional friend features:** The interface includes friend codes and activity sharing settings that can connect through a separately configured MoodMode server.

## Getting started

### Run the dashboard

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.
3. Start creating spaces and presets using the on-screen controls.

The main dashboard is a standalone HTML file with embedded CSS and JavaScript, so the basic interface does not require a build step or package installation.

### Optional social features

The friend and activity-sharing interface refers to a separate server started with:

```bash
node server.js
```

A `server.js` file and its setup instructions are not included in this HTML file alone. The optional social features will need the corresponding server implementation and configuration before they can be used.

## Data and privacy notes

- The dashboard stores much of its state in your browser's `localStorage`.
- Browser-local data is tied to the browser and device where it was saved; it is not automatically synced across devices.
- The interface includes optional activity sharing. Review the sharing settings carefully before enabling it, especially when using a shared server.
- Export important settings if you want a backup before clearing browser data.

## Project structure

```text
.
└── index.html   # Main MoodMode dashboard (HTML, CSS, and JavaScript)
```

## Deployment

You can host the static dashboard with GitHub Pages or another static website host:

1. Upload `index.html` to the root of your repository.
2. In the repository, open **Settings → Pages**.
3. Choose the branch you want to publish and select the root (`/`) folder.
4. Save the settings and wait for the deployment to finish.
5. Open the published URL shown in the Pages settings.

If you rename the file, keep the main page named `index.html` for the usual default behavior on static hosts.

## Limitations

- Features that depend on a separate server cannot work from the HTML file alone.
- Data stored in `localStorage` does not automatically follow you to another browser or device.
- Notifications depend on browser permissions and the page remaining open.
- Opening multiple links at once may be restricted by your browser's pop-up settings.

## Built with

- HTML
- CSS
- Vanilla JavaScript

## License

No license is specified yet. Add a license file if you want to define how others may use, modify, and distribute this project.
