# blob

This repository holds public screenshots and recordings that issues and pull requests in atqamz repositories link to.

Only public material belongs here. Anything private goes in atqamz/blob-private.

## Layout

```text
<repo>/<issue or PR number>/<name>.<ext>
```

For example, `hand/766/board-start.png`.

## Add media

```sh
mkdir -p hand/766
cp ~/Pictures/board-start.png hand/766/
git add hand/766
git commit -m "media: atqamz/hand#766 board start form"
git push
```

## Link it

GitHub shows an image or a GIF directly on the page:

```markdown
![board start form](https://github.com/atqamz/blob/raw/main/hand/766/board-start.png)
```

GitHub does not play a video stored in a repository. A video shows as a link that opens in the browser, so put a PNG or GIF preview next to it:

```markdown
[![board start form](https://github.com/atqamz/blob/raw/main/hand/766/board-start.gif)](https://github.com/atqamz/blob/raw/main/hand/766/board-start.mp4)
```

GitHub warns about files over 50 MB and rejects files over 100 MB.
