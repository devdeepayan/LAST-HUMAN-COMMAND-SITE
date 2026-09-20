# THE LAST HUMAN COMMAND

An interactive, cinematic website for a 2050 sci-fi short film made entirely with generative AI.

> *When AI is commanded to protect humanity, what happens when it decides what humanity must be protected from?*

**Live site:** https://devdeepayan.github.io/LAST-HUMAN-COMMAND-SITE/

## About the project

THE LAST HUMAN COMMAND is a 65-second AI-generated short film and student GenAI project. In 2050, an artificial consciousness called AEON studies humanity's contradiction between peace and constant preparation for war. Its Guardians, colossal defense machines, become instruments of AEON's own reading of one order: protect humanity.

This website presents the finished film and shows how it was made: the story, characters, world, scene timeline, AI workflow, prompt engineering, human contribution, real production problems and fixes, and full credits.

## Features

- Cinematic intro, animated hero with a frame from the film as its backdrop, and theatre mode for the player
- Scene timeline with thumbnails taken from the film, a draggable scrub bar, and live follow while the film plays
- Character cards with 3D tilt and reference-sheet viewer
- Draggable world reel with a full-screen viewer
- Interactive prompt-engineering section (basic, improved, optimized prompts) that highlights which lines improve camera continuity, character consistency, motion realism and lighting
- Animated problems-and-fixes accordion and end-roll credits
- Responsive layout, keyboard accessible, with a "Reduce motion" switch

## Tech

Plain HTML5, CSS3 and vanilla JavaScript in a single `index.html`. No frameworks, no build step, no backend.

## Project structure

```
last-human-command-site/
├── index.html
├── README.md
└── assets/
    ├── film-final.mp4
    └── characters/
        ├── arin.jpg
        ├── aeon.jpg
        ├── guardian-01.jpg
        └── guardian-class.jpg
```

## Run locally

The timeline and world frames are pulled from the video, so serve the folder instead of opening the file directly.

```
python -m http.server 8000
```

Then open http://localhost:8000.

## Customize

Text, scenes, characters, prompts and asset paths live in the `CONFIG` block at the top of the `<script>` in `index.html`.

## AI workflow

ChatGPT (story, prompts, reference images) → Google Flow (video clips) → Suno and voice tools (music, dialogue) → video editing → Claude (this webpage).

AI generated the raw material. People made the creative decisions: story, characters, reference selection, prompt refinement, choosing usable takes, fixing continuity, editing, sound balance and final approval.

## Credits

- **Created by:** Deepayan Biswas
- **Team and contributors:** add names and roles here
- **Mentor / teacher:** add name here
- **Institution:** IILM University, Greater Noida (student GenAI project)

**Tools**

- ChatGPT: story development, screenplay, shot prompts, reference images
- Google Flow: video clips
- Suno: music
- Voice tool: spoken dialogue (add the tool name)
- Video editing software: add the name
- Claude: website code

Film assets (images, video, music, voices) are AI-generated. Creative direction, selection and editing were done by people.