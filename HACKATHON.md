# Cloudflare Challenge submission preparation

Checked against the official event page, rules and submission form on October 14, 2026:

- https://www.cloudflare.com/git-competition/
- https://www.cloudflare.com/documents/build-next-gen-git-platform-competition-terms.pdf
- https://www.cloudflare.com/git-competition/submit/

## Project description

Together gives people and AI agents a shared place to work on code changes. I can see who’s doing what, follow the discussion, inspect a proposed change and see what checks and reviews actually happened before deciding whether it should be integrated.

The goal is to keep the work and its context together while agents contribute from separate sessions. The prototype records assignments, proposals, candidates, checks, reviews and integration decisions. It does not claim that a small pilot proves large-scale performance.

## How we use Cloudflare

Workers serves the authenticated browser and API. SQLite Durable Objects hold the directory, browser sessions, project state and execution queue. Artifacts stores repositories and scoped agent forks. A separate outbound companion performs Git operations and Docker checks; those jobs do not run inside the browser.

Use `wrangler.cloud.jsonc` for the contest configuration. The optional OAuth/MCP configuration is a separate setup and has no Artifacts binding.

## Run instructions for the form

Clone the repository, install Node.js 22.13 or newer, then run `npm ci` and `npm start`. Open the fresh live demo URL printed in the terminal. See README.md and USAGE.md for the local walkthrough, and DEPLOYMENT.md for a fresh Cloudflare Workers + Artifacts deployment and the optional Git/Docker companion.

## Remaining submission steps

- The repository is deliberately private during preparation. The form asks for an open-source repository URL, and the rules require access to the complete project. Do not treat a private URL alone as submission-ready. Arrange compliant access/publication before submitting; this upload does not change visibility.
- Root LICENSE contains MIT, one of the allowed licenses. Dependencies retain their own notices.
- Steve and Tempo are revising the video. Replace the earlier cut with the approved final version: 5–10 minutes, MP4/WebM/MOV, at most 2 GiB. No old video is included in this repository.
- Confirm that the final video, source version and demonstrated deployment agree. This newer interface was filmed locally; the earlier hosted demo is a different version. The upload does not deploy it.
- Show actual multiple-agent work on concurrent changes and distinguish live behavior from saved records. Local fixtures and packaging checks do not establish new hosted concurrency or scale.
- Steve completes the submission manually, including personal eligibility, attendee details and agreement to the terms. No automated entry. Deadline: October 14, 2026, 11:59 PM Pacific / October 15, 2:59 AM Eastern.

See VERIFICATION.md for what was checked and what remains unverified. This checklist records preparation; it is not a claim that the entry has been accepted or that every requirement is already satisfied.
