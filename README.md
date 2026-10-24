# The AI Seven

A playful, practical field guide to seven everyday AI skills for higher education professionals. Each skill has a plain-language explanation, a campus example, a fill-in-the-blank prompt to copy, and a small hands-on lab.

**Live site:** https://wangy113.github.io/the-ai-seven/

Link straight to one skill by adding `#skill-1` through `#skill-7` to the address, for example https://wangy113.github.io/the-ai-seven/#skill-5.

## What's in the repo

| File | What it is |
| --- | --- |
| `index.html` | The whole site: page, styles, and script in one file. No build step. |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and home-screen icons. |
| `social-card.png` | Preview image shown when the link is shared in Teams, Slack, or email. |

## Editing the content

Everything editable lives near the top of the `<script>` in `index.html`:

- **`MODELS`**: the model names (Claude Sonnet 5.5, GPT-6, Gemini, and so on). Model names change often; update them here and every mention on the page follows.
- **`skills`**: the seven skills. Each has a title, definition, example, tiny move, watch-out, and prompt. Words in `[brackets]` inside a prompt become fill-in blanks on the page. Brackets that start with "paste" (like `[paste code]`) stay as plain text, because that material goes straight into the AI chat.
- **`MODEL_TASKS`**: the choices and advice in the Model matcher lab.
- **`HTML_FIX`**: the broken and fixed HTML in the Canvas repair lab, with the numbered list of what is wrong.

The model advice follows BoodleBox's [Choose a model](https://help.boodlebox.ai/article/choose-a-model) guide. Check it when you refresh the examples.

## Design rules

- **Four type sizes only**, set as tokens at the top of the stylesheet: small 15px (labels, buttons, notes), body 18px (reading text), title 26px (22px on smaller screens), and display (page and section headings). Nothing is smaller than 15px. Use one of the four tokens rather than adding a new size.
- The cream "groovy" palette is intentional (see `.impeccable/config.json`).

## Privacy

Nothing on the page sends data to an AI service. What people type into the prompt blanks stays in the browser tab and is never saved. The only thing stored is which skills a visitor has marked as tried, kept in that browser's local storage.

## Publishing

GitHub Pages serves the `main` branch, so pushing to `main` updates the live site within a minute or two.
