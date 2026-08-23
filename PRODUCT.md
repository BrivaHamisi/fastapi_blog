# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Primary readers: general public visitors interested in FastAPI and Python web development. Secondary user: the developer building the site as a hands-on learning exercise; their success is understanding FastAPI, not shipping a polished commercial product.

## Product Purpose

A blog for publishing short posts about FastAPI and Python web development, built by adapting Corey Schafer's well-known blog tutorial from Flask to FastAPI. Success means: the tutorial concepts work end to end, and the resulting site is presentable enough that a public visitor has a coherent reading experience.

## Positioning

A faithful FastAPI adaptation of a widely-followed Flask tutorial — its value is the port itself and the learning trail, not competitive features.

## Operating Context

- Follows Corey Schafer's blog tutorial structure (templates, sidebar, styling conventions descend from it).
- Runs locally with uv-managed Python 3.13 and uvicorn/FastAPI CLI (`main:app`).
- Data lives in memory and resets on every restart; there is no database yet.

## Capabilities and Constraints

- Home/post listing served at `/` and `/posts`; JSON API at `/api/posts` and `/api/posts/{id}`.
- `templates/post.html` (detail view with edit/delete affordances) exists but no route serves it yet.
- Authentication is planned but not implemented: Login/Register nav buttons are placeholders; TODOs mark authorization work in `post.html`.
- Posts are a hardcoded in-memory list of two sample entries; content is placeholder copy, not real articles.
- Frontend stack: Jinja2 templates, Bootstrap 5.3.8 via CDN, Google Fonts (Montserrat/Nunito), light/dark/auto theme toggle persisted in localStorage, PWA manifest and icon set.
- Explicitly undecided: database choice, real post authoring flow, deployment target.

## Brand Commitments

- Site name: **FastAPI Blog** — binding.
- Footer credit: **Briva Digital** ("© Briva Digital. All rights reserved.") — binding.

## Evidence on Hand

- Two sample posts defined in `main.py` (authors "Corey Schafer", "Jane Doe") — placeholder content, not real articles.
- Default profile picture (`static/profile_pics/default.jpg`) and complete favicon/PWA icon set (`static/icons/`).
- Absences future work must not fabricate: no real posts, testimonials, metrics, or deployment claims exist anywhere in the repo.

## Product Principles

1. **Learning is the point.** Code stays readable and tutorial-shaped; clarity outranks cleverness.
2. **Honest scaffold.** Anything shown as functional must actually work, or read as clearly planned (TODO); never present placeholder content as real.
3. **Public-presentable.** Even as a tutorial project, any page a stranger lands on should feel coherent and finished.
4. **Respect the names.** "FastAPI Blog" and "Briva Digital" appear exactly as committed.
5. **Room to grow.** Structure anticipates the planned additions (post detail routing, authentication) rather than working against them.
