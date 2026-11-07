# Journal of Applied Memetics

**Memes for academia.** Ready-to-use memes for scientific talks, built only on public-domain and openly licensed images. Pick one, change the text, and download it as a PNG with the image credit already in the corner.

The site is a single static page (`index.html`) that reads the library from `data/memes.js`. Submissions arrive as GitHub issues; when a maintainer accepts one, a workflow adds the image and its credit to the repository and redeploys the site.

## Set up

1. Create a public repository (for example `applied-memetics`) and push these files to the `main` branch.
2. **Settings → Pages → Build and deployment → Source: GitHub Actions.** The `Deploy site` workflow publishes the site on every push.
3. **Issues → Labels:** create two labels, `submission` and `accepted`.
4. If you use a custom domain, set `JAM_REPO` near the top of the script in `index.html` to `your-username/your-repo`. On `*.github.io` the repository is detected automatically.

If the publish workflow fails with a permissions error, check **Settings → Actions → General → Workflow permissions** and allow read and write. If `main` is protected, allow GitHub Actions to push to it.

To try it locally, open `index.html` in a browser. The gallery images load from Wikimedia Commons, so you need to be online.

## The starter library

The twelve starter memes are built on public-domain paintings (Friedrich, Caravaggio, Géricault, Bruegel, Munch, Rembrandt, David, Hokusai, Titian, Vermeer) and public-domain NASA images. The images are loaded from Wikimedia Commons, and each meme links to its Commons page. Famous meme templates such as Drake or Distracted Boyfriend are not here, because their images are copyrighted and not openly licensed.

## How submissions work

1. Someone makes a meme from their own photo or an openly licensed image and clicks **Open submission on GitHub** on the site, which opens the prefilled form in `.github/ISSUE_TEMPLATE/submit-meme.yml`.
2. They drag the image in, state the image licence, creator and source link, and submit. The issue gets the `submission` label.
3. A maintainer checks the joke and the licence, then adds the `accepted` label.
4. `.github/workflows/publish-meme.yml` runs `.github/scripts/ingest_meme.py`, which downloads the image, saves it as `memes/JAM-XXXX.ext`, appends the entry to `data/memes.js`, commits, redeploys the site and closes the issue with a thank-you.

To reject a submission, close the issue with a kind comment.

## Entry format

Starter memes (caption drawn over a Commons image):

```json
{
  "id": "JAM-0011",
  "top": "Revising the paper",
  "bottom": "round four",
  "slot": "Limitations",
  "tags": ["reviewers", "writing"],
  "work": "Sisyphus",
  "creator": "Titian",
  "year": "1548–49",
  "licence": "Public domain",
  "img": "https://upload.wikimedia.org/.../960px-Punishment_sisyph.jpg",
  "hires": "https://upload.wikimedia.org/.../1280px-Punishment_sisyph.jpg",
  "source_url": "https://commons.wikimedia.org/wiki/File:Punishment_sisyph.jpg"
}
```

Submitted memes (finished image stored in the repository):

```json
{
  "id": "JAM-0013",
  "title": "When the robot works in simulation",
  "slot": "Results",
  "image": "memes/JAM-0013.png",
  "licence": "CC BY-SA",
  "creator": "Jane Doe",
  "source_url": "https://commons.wikimedia.org/wiki/File:...",
  "contributor": "@someone"
}
```

Parts of the talk: Title, Motivation, Related work, Methods, Demo, Results, Limitations, Future work, Q&A, Acknowledgements.

## Content policy

Every image must be public domain, openly licensed for reuse, or the submitter's own. Each meme carries its credit, and downloads keep it in the corner. Punch up, never down.
