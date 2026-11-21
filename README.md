# Databricks learning tools

This site collects browser-based activities for learning Databricks. Visitors can open the listed activities without a Databricks or GitHub account.

- [Open the learning tools homepage](https://jamesl-databricks.github.io/)
- [Play or host Databricks Bingo](https://jamesl-databricks.github.io/databricks-bingo/)

## Preview locally

From the repository root, run:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/). The homepage uses plain HTML and CSS. The Bingo link points to a separately deployed GitHub Pages project and is verified on the published site.

## Add an activity

Add a card to `index.html` with the activity name, a short description, and its public HTTPS link. Use a root-relative link such as `/databricks-bingo/` for projects served on this hostname. Verify the activity in a signed-out browser at desktop and mobile widths, and check that the launch link works with the keyboard. Link to public entry pages and keep private session links and credentials out of the catalog.

## Publish

The homepage files are at the root of `main`. For a branch deployment, set GitHub **Settings → Pages** to **Deploy from a branch** and select **main** and **/ (root)**. Keep `.nojekyll` so Pages serves the static files directly.

After pushing a site change, check the Pages deployment in **Actions**. Open the public homepage over HTTPS in a signed-out browser and follow each activity link.
