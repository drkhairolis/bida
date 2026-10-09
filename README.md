# BPMNK2033 – Interactive lecture slides

```
bida/
├── index.html            ← course landing page (list of chapters)
├── chapter1/
│   └── index.html        ← Chapter 1: Introduction to Business Analytics
├── chapter2/
│   └── index.html        ← Chapter 2: Basic Excel Formulas & Functions
├── chapter4-5/
│   └── index.html        ← Chapters 4 & 5: Data Visualization & Exploration (2 lectures)
└── README.md
```

Every chapter is one self-contained HTML file. You don't need to install or build anything.

## Publish on GitHub Pages (about 10 minutes, first time only)

1. Sign in at **github.com** (or create a free account). Your username becomes part of the link.
2. Click **+ → New repository**. Name it **`bida`**, set it to **Public**, and click **Create repository**.
3. On the new repo page, click **uploading an existing file**. Drag in **everything inside this folder**: `index.html`, `README.md` and the whole `chapter2` folder. Then click **Commit changes**.
4. Go to **Settings → Pages**. Under *Build and deployment*, set **Source: Deploy from a branch**, **Branch: `main`**, folder **`/ (root)`**, then click **Save**.
5. Wait 1–2 minutes and refresh the Pages settings. Your site will be live at:
   - Landing page: `https://<your-username>.github.io/bida/`
   - Chapter 2: `https://<your-username>.github.io/bida/chapter2/`

Deep links work too. For example, `…/chapter2/#18` opens the VLOOKUP slide directly.

## Add the next chapter

Create a folder such as `chapter3/`, put its `index.html` inside it, upload the folder (**Add file → Upload files**), and edit the card in the landing page `index.html` so it links to the new folder.

## Use it on the Google Site

In Google Sites, choose **Insert → Embed → By URL** and paste the Chapter 2 link. You can also add a button that links to it.

## Presenting

| Key | Action |
|---|---|
| → / Space / PageDown | Next slide |
| ← / PageUp | Previous slide |
| M | Slide menu |
| F | Full screen |
| T | Start or pause the 70-minute lecture timer (double-click the timer to reset it) |

On phones, the slides stack into one scrolling page so students can follow along.

## Editing the dataset

Near the top of the `<script>` block in `chapter2/index.html`, find `const DATA = [...]`. Each row is `[Rank, Make, Model, Sales 2021, Sales 2020]`. Replace these rows with the figures from your class `top20vehicles2021` file, and every demo, lookup and highlight will update automatically. Check the quiz explanations afterwards: the IF question uses the F-Series figures, so update that text if the numbers change.

## Chapters 4 & 5 (two lectures in one module)

`chapter4-5/index.html` has 32 slides. **Part A (Chapter 4)** is slides 1–18 and **Part B (Chapter 5)** is slides 19–32. For the second lecture, open `…/chapter4-5/#19`. The timer starts from 00:00 when you move past slide 19; double-click it to reset at any time.
