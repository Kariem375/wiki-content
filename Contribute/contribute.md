# Want to Contribute?

Use this page to submit content updates to the wiki through GitHub pull requests.

[Open the wiki-content repository](https://github.com/BritPVE/wiki-content)

## How To Submit a PR

1. Fork `BritPVE/wiki-content` to your GitHub account.
2. Create a new branch for your change.
3. Choose the relevant top-level folder (for example `Wiki/`) and edit or add the target `.md` file.
4. Commit with a clear message describing what changed.
5. Open a pull request to `BritPVE/wiki-content:main`.
6. Include a short summary in the PR description.

## How Navigation Works

The wiki menu is controlled by `navigation.json` at the root of the wiki-content repo. Page files are discovered automatically, but **they will not appear in the menu until you add them to `navigation.json`**.

When adding a new page:

1. Add your `.md` file to the repo (for example `Wiki/my-new-page.md`).
2. Open `navigation.json` and add the page slug to the correct category's `pages` array.
3. Use the filename slug (for example `my-new-page`) or the file path (for example `Wiki/my-new-page.md`).
4. Order pages in the array as you want them to appear in the side menu.

Example category entry:

```json
{
  "name": "Guides",
  "pages": [
    "beginner-guide",
    "my-new-page"
  ]
}
```

To hide a page from the menu without deleting it, add its slug to the `hiddenPages` array in `navigation.json`.

## Quick Formatting Tips

- You can find a helpful guide on markdown [here](https://www.markdownguide.org/cheat-sheet/)
- Use one `# Title` at the top of each markdown page.
- Use headings and bullet points to keep pages readable.
- Keep content accurate and concise.
