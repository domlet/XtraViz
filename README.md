# XtraMath Dashboard — GitHub Pages (local CSV)

A static HTML/JavaScript dashboard. **No server, Node.js, packages, or CSV in the repository are required.**

## Deploy

1. Create a GitHub repository.
2. Upload `index.html` and `.nojekyll` to the repository root. **Do not upload real student CSVs.**
3. Go to **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
4. Open the published Pages URL. Select your XtraMath CSV using **Choose File**.

## Supported CSV format

XtraMath exports with columns `code_name`, `Operation`, `Placement Fluency Score`, `Current Fluency Score`, `Number of Quizzes`, optionally `Class`/`Section`. Supports grouped exports with single-cell section header rows, and operation labels such as `Addition (3s)`. Quoted CSV fields and UTF-8 are supported.

## Privacy

The CSV is read using the browser's File API. There are no network requests in the app. The selected CSV and student data are **not uploaded** or saved to GitHub. The page does not retain data after refresh. Anyone with the public link can access the dashboard code, but not your locally selected file.

## Rankings

Progress leaderboard: furthest operation reached, then fluency score at that operation. Growth & practice: 70% percentile ranking of summed score improvements, 30% percentile ranking of quiz volume. Quizzes are a proxy for activity, **not verified daily practice consistency**.
