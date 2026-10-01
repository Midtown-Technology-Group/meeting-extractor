# Repository guidance

This repository is an initialized placeholder for a Microsoft 365 meeting-extraction tool. `README.md` describes planned transcript, note, recording-metadata, action-item, and summary functions; those plans are not implemented capabilities. The current default branch contains no application build/test configuration or CI workflow.

Before starting implementation, agree the first supported input and observable output with the user. Inspect the current tree and README again rather than assuming a language, framework, authentication mechanism, Microsoft Graph permission set, or deployment path has already been selected. Record those decisions in the smallest useful repository document as the code is introduced.

The intended related tools are `calendar-glance`, `todo`, and `mail-triage`; links in `README.md` are navigation pointers, not proof of a working integration. Verify the exact integration contracts before coupling this project to another toy.

Use synthetic meeting content for initial tests. Real transcripts, recordings, participant details, and follow-up tasks can contain customer or personal data: keep credentials and raw meeting content out of source and debug logs. Reading Microsoft 365 content and creating or sending follow-ups are separate operations requiring their own authorized scope.

Do not invent verification commands for an empty scaffold. Once a runnable slice exists, add a documented local check and CI command at the same time, and report what was actually exercised. Preserve the GPL-3.0-or-later license noted in the README.
