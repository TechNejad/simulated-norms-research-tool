# Simulated Norms Research Tool

This repository contains a single‑page application for collecting and analyzing data about research papers in the Simulated Norms project. The tool is built with plain HTML, CSS and JavaScript and is designed to run entirely on the client side. You can use it locally or host it via GitHub Pages.

## Features

- Add, edit and delete entries for research papers
- View aggregate statistics and distribution charts on the dashboard
- Filter and search your entries in the browser tab
- Export a summary of your data

## Data Storage

By default, all data is stored in your browser's `localStorage`. This allows offline use and quick access on the same device. However, `localStorage` does not sync across browsers or devices. There is no longer any external dependency (such as Google Sheets) in this version of the tool.

If you wish to back up or share your data, use the **Export** tab within the application. You can export your entries to either JSON (`thesis_data.json`) or CSV (`thesis_data.csv`). The exported file will contain all of your papers in a simple text format.

To persist your data in the repository itself, download the CSV export and commit it to this repository (for example, add it as `data/thesis_data.csv`). Subsequent exports will reflect any new entries you add. Because this project runs entirely in the browser, there is no automated commit – manual uploads give you full control over when your data is published.

### Running Locally

Simply open `index.html` in your web browser to start using the tool. No build step is required. For the best experience on GitHub Pages, rename `thesis-tool.html` to `index.html` or set your GitHub Pages source accordingly.

### Hosting on GitHub Pages

1. Commit the files in this repository to GitHub.
2. In your repository settings, scroll to **Pages** and choose the source branch (e.g. `main`) and folder (e.g. `/root` or `/docs`).
3. Save the settings. GitHub will build and serve your site at `https://<username>.github.io/<repository>/`.

## License

This project is provided without any warranty. Feel free to use and modify it for your research or educational purposes.
