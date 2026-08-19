<p align="center">
  <img src="assets/valley-ai-symbol.png" alt="The Valley AI Club" width="120">
</p>

# The Valley AI Club

**Learn AI. Build together. Serve the Valley.**

The Valley AI Club is a youth-led AI community for middle school and high school students across the San Fernando Valley. We provide a welcoming place to understand how AI works, build useful projects, and explore how technology can support local people and communities.

No coding or AI experience is required—curiosity is enough.

[Visit the website](https://valley-ai-club.github.io/) · [Join the club](https://forms.gle/at6Uc2pfSiB53pCx8)

## Who can participate

- Students in grades 6–12
- College students interested in mentoring
- Students at any experience level

## What we explore

### AI for Health & Data Science

Explore health data, prediction, and responsible AI to spot patterns and ask better questions.

### Coding, Simulation & Robotics

Learn programming by modeling real systems, testing ideas, and connecting code to the physical world.

### AI for the Valley Community & Environment

Build locally meaningful projects around community needs, the environment, and everyday life in the Valley.

## Upcoming events

### AI in Health: Student Journeys and Future Pathways

A student panel on college applications, summer research, and what comes next, hosted with the CHEER Youth Group.

- **When:** Wednesday, August 19, 4:00–5:30 PM PDT
- **Where:** Online via [Zoom](https://ucla.zoom.us/j/99291870470)
- **Opening remarks:** UCLA Fielding School of Public Health Senior Associate Dean
- **Panelists:** Aaron (MIT 2030), Arin (Stanford 2028), Royce (MIT 2030), Siray (Columbia 2029), Sophia (Stanford 2029), Vincent (Caltech 2030)

## Planned activities

- **AI workshops:** friendly, hands-on introductions for students at any experience level
- **AI camps:** longer sessions to go deeper on a theme with mentors alongside you
- **Datathons:** explore real datasets, form questions, and communicate discoveries
- **Hackathons:** design and build useful AI-powered projects in teams
- **Codathons:** practice programming through focused challenges and peer support

## Mentorship and community

The club is led by high school students and guided by UCLA faculty and student mentors with experience in Data Science and AI for Health education. We work in collaboration with CHEER.

> The Valley AI Club is a community initiative and does not represent an official UCLA program.

## About this website

This repository is the club's website, built with [Jekyll](https://jekyllrb.com/)
and hosted on GitHub Pages. GitHub builds the site automatically on every push to
`main` — there is no build step to run yourself.

```text
.
├── _config.yml         # Site settings, navigation, collections
├── _data/
│   ├── themes.yml      # The three themes (name, blurb, photo, accent colour)
│   └── activities.yml  # Workshops, camps, datathons, hackathons, codathons
├── _events/            # One markdown file per event
├── _includes/          # Header, footer, event cards, join CTA
├── _layouts/           # default, page, event
├── index.html          # Home
├── events.html         # Events calendar
├── about.html          # About
├── join.html           # Join
├── 404.html
└── assets/             # Styles, images, and fonts
```

### Adding an event

Create a file in `_events/` named `YYYY-MM-DD-short-name.md`:

```yaml
---
title: "Your event title"
subtitle: A one-line description
date: 2026-09-15 16:00:00 -0700
time_label: 4:00&#8211;5:30 PM PDT
theme: health          # health, code, or valley — see _data/themes.yml
location: Online via Zoom
host: the CHEER Youth Group
join_url: https://example.zoom.us/j/000000
panelists:
  - name: First name
    school: School 2030
---

Anything written below the front matter becomes the body of the event page.
```

The event appears automatically on the home page and the events calendar. Events
move from "Upcoming" to "Past events" based on their date, and each is tagged with
one of the three themes so the calendar can be grouped by theme once there are
enough events to make that useful.

Two things to know:

- `future: true` is set in `_config.yml`. Without it, Jekyll treats an event dated
  in the future as an unpublished draft and never builds its page.
- The upcoming/past split is decided when the site is built. GitHub rebuilds on
  every push, so an event that has just passed moves to "Past events" on the next
  push.

### Previewing locally

Requires Ruby 3.x (macOS system Ruby 2.6 is too old for current Jekyll):

```bash
bundle install
bundle exec jekyll serve
```

Then open [http://localhost:4000](http://localhost:4000).

## Get involved

Interested in learning, building, mentoring, or contributing?

- [Complete the interest form](https://forms.gle/at6Uc2pfSiB53pCx8)
- Email [sfvalleyaiclub@gmail.com](mailto:sfvalleyaiclub@gmail.com)
