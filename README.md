# Explore the Performance page: interactive walkthrough

A short, top-level walkthrough of the Performance page in MomentusMAX. A screen sits on the left and short, large-print notes sit on the right, in the same layout as the Today's Focus, Opportunity page, Calendar, and Tasks walkthroughs.

## What learners do

- Start on an overview and select a numbered area on the screen, or use Next and Back.
- On Rep and Manager views, select Rep View or Manager View to see each one.
- On Health metrics, select Monthly or Yearly.
- On the chart steps, select a label to zoom to that chart.

Steps: Overview, Rep and Manager views, Event type, Health metrics, New opportunities, Stage charts, Active holds, Leaderboard, Manager View.

## Repo contents

| Path | Purpose |
| --- | --- |
| `index.html` | The walkthrough. Screens, scripts, and styles are inlined. The only external request is Google Fonts, which falls back to system fonts |
| `.nojekyll` | Tells GitHub Pages to serve the file as is |
| `.gitignore` | Standard ignores |

## Run locally

Open `index.html` in a browser.

## Publish with GitHub Pages

1. Push to `main`.
2. In the repo, go to Settings > Pages, choose Deploy from a branch, then `main` and `/ (root)`.
3. The page is served at `https://<user>.github.io/<repo>/`. Suggested repo name: `MAX-performance-nav`.

## Embed in Genially or 360Learning

The page is responsive. Give it as much room as you can, ideally a full slide.

```html
<iframe src="https://<user>.github.io/<repo>/" title="Explore the Performance Page Walkthrough" width="100%" height="100%" style="border:0;width:100%;height:100%;" allowfullscreen loading="lazy"></iframe>
```

Test in Genially's Preview or published view. Embeds can look blank in the editor.

## How it was built

The four screens are full-length renders of saved snapshots of the Performance page (Rep View monthly, Rep View yearly, the Event Type menu, and Manager View yearly). The page scrolls, so each render shows the whole page, not just the first screen. The left navigation bar is not included. The top bar is kept. Nothing was redrawn.

- **Manager View** is cut off above its General Performance section.
- **Rep names:** in Manager View the rep names are baked into the chart images, so they are pixelated instead of replaced.
- **Not used:** the snapshot of the Rep menu (it lists test usernames) and the second Event Type snapshot (a duplicate of the first).

To change notes, edit the `STEPS` array in `index.html`. To change a screen, use a new approved capture. Do not edit the embedded images.

## Sources for the notes

| Step | Source |
| --- | --- |
| All steps | Labels and values shown on the captured screens |
| Health metrics, New opportunities, Stage charts, Leaderboard | The explanations of what each chart means are inferred from the chart titles and need Product to confirm |
| Manager View, Total pipeline | The note under the chart title: active pipeline only, excluding Closed Won, Closed Lost, and Not Qualified |

## Before you publish

- Product to confirm the inferred explanations listed above.
- The demo data shows some unfinished labels, such as "Average Deal Size (null)", "Current Rep: null - Rank #null", and several "No data" panels. They are shown as captured. Recapture with fuller demo data, or tell me to mask them.
- Product or Security must confirm the demo data is mock.
- This file contains captures of the MomentusMAX interface and is Momentus internal training content. Keep the repo private unless Momentus approves public sharing. No license is granted. All rights reserved by Momentus Technologies.
