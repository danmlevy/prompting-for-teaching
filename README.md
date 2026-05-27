# Prompting for AI in Teaching

This repository contains the GitHub Pages site for the reusable faculty learning module, "Prompting for AI in Teaching."

Live site:
https://danmlevy.github.io/prompting-for-teaching/

## Current Files

- `index.html` - the live GitHub Pages page. It contains the HTML, CSS, small copy-button script, participant text areas, and the embedded PingPong Prompt Coach iframe.
- `bot-system-prompt.md` - the recommended system prompt/instructions for the PingPong Prompt Coach.
- `README.md` - project notes for future editing.

There is not currently a separate Markdown source file. If you later want an easier-to-edit text source, create `source.md` and treat `index.html` as the published version.

## Bot Embed Location

The PingPong bot is embedded in `index.html` in section 6, "Get Feedback from the Prompt Coach."

Search for:

```html
<iframe
  class="assistant-frame"
  title="PingPong Prompt Coach"
  src="https://pingpong.hks.harvard.edu/group/39/shared/assistant/3517?share_token=019e3bb9-3598-7673-857d-4425ac2785ed"
```

The same PingPong URL also appears immediately below the iframe as a fallback "open it in a new tab" link.

## Editing Guidance

Keep the page practical, supportive, intellectually serious, and not hypey. The required experience should take about 20 minutes, with optional extensions up to about 45 minutes.

The page should stand alone as a general faculty module on prompting for teaching. Put occasion-specific instructions, such as "please complete before our seminar," in the participant email or invitation rather than hard-coding them into the page.

The core teaching frame is TIC:

- Task: What do you want the AI to do?
- Instructions: How should the AI do it?
- Context: What does the AI need to know?

When updating either the page or the bot, keep the language consistent around these ideas:

- Good prompting is iterative.
- Participants are practicing, not being graded.
- The Prompt Coach should coach the prompt before answering the underlying teaching task.
- Feedback should be concise enough that participants actually revise.
- The experience should prepare participants for later AI projects, custom GPTs, or reusable teaching tools.
- Section 9 includes a completion survey link: https://forms.gle/nnZ7uhXR2ydXVe8u6

## Local Preview

The site is a single static HTML file. To preview it locally, open `index.html` in a browser.

You can also run a tiny local web server from this folder:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Publishing

The live site is published by GitHub Pages from the `main` branch. After editing and checking the page locally, commit the changes and push to GitHub. GitHub Pages should update automatically after the push.
