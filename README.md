# CloudCannon Headless CMS Demo

This repo illustrates one approach to building a git-based headless CMS using CloudCannon.

The files in the `content` are used as the site, and are passed through the CloudCannon build unchanged.
As these files are JSON files, this means they can be accessed as if they were an API endpoint — for example
the file at `content/posts/hello_world.json` could be loaded at `https://<website_address>/posts/hello_world.json`.

When editing in CloudCannon, these posts will open in the Visual Editor, using the preview page found at `content/previewer/index.html`. This file uses CloudCannon's live editing APIs to fetch the relevant data on load, and previews the content of the JSON file with some hypothetical styling to match the end consumer application.
