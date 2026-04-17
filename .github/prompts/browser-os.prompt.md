---
description: "Run the browser OS benchmark prompt against the current model. Save the output as browser-os.html under a folder named after the model used, then commit."
argument-hint: "Model folder name (e.g. 'claude-sonnet-4-5', 'gpt-5', 'gemini-2-5-pro')"
mode: agent
tools: [edit, execute]
---
Using html, css and js, generate a browser OS with the following features:
- At least 5 applications
- Two of the 5 applications must be FUNCTIONAL 3d games. One must be a simple GTA clone, and another can be up to you.
- Ability to change wallpaper
- A "special" feature that you decide on and document what it is & why it is special.
The result must be contained within a single script, and be able to be opened in Chrome browser.
this will be your only attempt. after this plan, we will be build what you plan here.

---

## After generation

1. Save the complete generated HTML to `{{model-folder}}/browser-os.html`
2. Run: `git add {{model-folder}}/browser-os.html && git commit -m "feat: add {{model-folder}} browser-os"`
