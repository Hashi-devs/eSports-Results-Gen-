# Match Day Studio

Results graphics for esports tournaments, from any game. Upload your finished design once, let the app find where the results go, then fill it in (or import the results) and download the graphic at full quality.

## What it does

- **Your designs only.** Every user uploads their own templates. Nothing is shared between users: templates, teams and fonts are saved in the user's own browser.
- **Finds the spots for you.** Upload a design and the app looks for repeated table rows and works out the columns from:
  - placeholder text such as `-`, `00`, `XX`, `TEAM NAME` or `TBD` (it removes them from the background),
  - empty cells lined up under your column headers.
  Things printed in the design that change row to row, like rank numbers, are left alone.
- **Mark spots by hand** for anything else: team names, short tags, logos, pictures, text and numbers, each with its own font, weight, size, colour and alignment.
- **Teams library** with logos. Add many at once from logo files named after each team.
- **Import results** from Excel, CSV/TSV, Google Sheets downloads, JSON or pasted text, as final standings or match by match. Match-by-match results are added up with editable scoring rules (points per kill, placement points table).
- **Auto total and sorting** (for example Total = KP + PP, sorted high to low).
- **Many graphics at once** from one table, downloaded as a zip.
- **Garet** (Book and Heavy) is built in. Upload any other fonts in the Fonts tab.

## Running it

It is a static site with no build step: `index.html` plus the `fonts` folder.

### Deploy on Vercel

1. On vercel.com choose **Add New → Project** and import this repository.
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy. Every push to `main` deploys again automatically.

### Run locally

Open `index.html` in a browser, or serve the folder with any static server (for example `npx serve .`).

## Font licence

Garet is a free font by Spacetype. Its licence allows embedding it in websites and apps, including commercial ones, but not redistributing the font files on their own. See `Spacetype EULA` in the original download.
