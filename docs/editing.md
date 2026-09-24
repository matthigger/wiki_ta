# Editing this wiki

Every page is a Markdown file in the `docs/` folder of the
[wiki_ta](https://github.com/matthigger/wiki_ta) repo. The site
rebuilds automatically a minute or two after each change to `main`.

## Edit a page in the browser

1. Click the pencil icon at the top right of the page.
2. Make your change in GitHub's editor; use the Preview tab to check it.
3. Click **Commit changes**. If you don't have write access, GitHub offers
   to open a pull request instead, which the instructor will review.

## Add a page

1. Create a new `.md` file under `docs/` (subfolders are fine).
2. Add it to the `nav:` list in `mkdocs.yml`, or it won't appear in the
   sidebar.

## Markdown cheat sheet

| You type | You get |
|---|---|
| `# Title`, `## Section` | headings |
| `**bold**`, `*italic*` | **bold**, *italic* |
| `- item` | bullet list |
| `1. step` | numbered list |
| `- [ ] task` | checkbox |
| `[text](other_page.md)` | link to another page |
| `` `code` `` | `code` |

Callout boxes:

```markdown
!!! warning
    Don't release grades before the regrade window closes.
```

!!! warning
    Don't release grades before the regrade window closes.

## Preview locally (optional)

```bash
pip install -r requirements.txt
mkdocs serve
```

then open <http://127.0.0.1:8000>.
