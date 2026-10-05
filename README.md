# Videobolt Content Lab

A shared workspace for coming up with video ideas and turning them into scripts. It lives in `content-lab/index.html` and is published as a claude.ai artifact.

It has five sections:

1. **Brand bible**: voice and tone, words to use and avoid, audiences, content pillars, series, account personas, CTAs and reference scripts. Every prompt in the tool reads from it.
2. **Teardowns and pattern library**: add a reference video's transcript, screenshots and numbers to get the hook, structure, craft, a performance read and Videobolt adaptations. Hooks and structures it finds are saved to a library you can reuse.
3. **Market watch**: competitor profiles, a form for logging posts (each gets an ignore, counter or borrow suggestion), weekly digests and a shift log.
4. **Concepts**: generate concepts from a brief (series, platform, goal, persona, hook, template, pattern), then save, rate, annotate and set a status on each.
5. **Scripts**: a beat outline, full script (VISUAL / ON-SCREEN / VO), shot list and captions, each editable and approved before moving on. Also includes a brand check, read time at your speaking pace, a teleprompter and a Markdown export.

The page stores its data in the artifact's shared database. Collections: `brand/bible`, `teardowns`, `patterns`, `competitors`, `watch`, `digests`, `shifts`, `concepts`, `scripts`. Generation runs inside the page on the viewer's own Claude account. Opened outside claude.ai, the page still works as a workspace and saves to the browser only.

The automatic weekly competitor check writes into `digests` (with `source: "scheduled"`) and `shifts`.
