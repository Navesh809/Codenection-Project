# NHSY

**Group trip planning, without the group chat arguments.**

Built for **CodeNection 2026** — Lifestyle & Personal Productivity track, "Planning an Escape" — by team *Works on my pc*.

---

## Overview

NHSY is a group trip-planning app built on the idea that a trip isn't a fixed plan — it's a living one. Today, group trips get coordinated across five different apps and an endless group chat: flights, budgets, itineraries, and everyone's preferences are scattered, there's no structured way to see where the group actually agrees, and when something goes wrong mid-trip (a delayed flight, a closed venue) there's rarely any real help getting back on track.

NHSY brings all of that into one place: it blends everyone's preferences into a single AI-built itinerary, keeps a live shared budget, and turns disruptions into a quick swipe-and-vote instead of a group-chat scramble.

## The Problem

- **Endless group-chat debates** — no structured way to see where everyone actually agrees.
- **"Who owes what?"** — budget tracking lives in a separate app, if it exists at all.
- **No plan B** — a delayed flight or closed venue derails the whole trip, with no built-in recovery path.

## How We Got Here

Three sub-concepts were tested against the "Planning an Escape" brief before landing on NHSY:

| Concept | Core Idea | Outcome |
|---|---|---|
| **NHSY** | Group vibe-matching + AI itinerary + live budget + disruption swipe deck | **Chosen** — covers all four pillars of the brief |
| Wingman | Overlap finder for solo travellers' independent itineraries | Set aside — no shared budget or itinerary |
| DriftPlan | Buffer-based itinerary engine with auto-cascading reschedules | Set aside — weak on group preference sync |

## Core Features

| Feature | What it does |
|---|---|
| **Trip Blend** | A visible compatibility score across the group, before anyone has to argue about it. |
| **AI Planner** | One itinerary built from everyone's budget and interests. |
| **Split Cost** | Budget auto-splits per person and updates as plans change. |
| **Re-plan** | Flight delay or closed venue? Swipe through alternatives, vote, done. |
| **Live Mode** | Real-time alerts and today's plan while the trip is happening. |

## How It Flows

Eight screens, one clear path:

- **Account setup:** Login → Profile → Create Trip → Quiz
- **Core planning flow:** Blend → Explore → Dashboard
- **Overlays** (open on top of the flow, return to their parent screen): Alternatives, Re-plan

## What Makes It Different

- **Blend (after the quiz):** a visible % match score across the group; conflicts are flagged instead of buried; swipe to resolve preference clashes.
- **Re-plan (mid-trip disruption):** a persistent banner when something changes; swipe through 2–3 alternatives; the group votes and the Dashboard updates live.

### Competitive Landscape

| | NHSY | Wanderlog | TripIt | Splitwise |
|---|:---:|:---:|:---:|:---:|
| Group preference blending | ✓ | — | — | — |
| Live disruption re-planning | ✓ | — | partial | — |
| Budget + itinerary combined | ✓ | partial | — | budget only |
| Real-time group voting | ✓ | — | — | — |

## Tech Stack

| Layer | Tool |
|---|---|
| Frontend + API routes | **Next.js** |
| Database + Realtime | **Supabase** (Postgres + Realtime) |
| Hosting | **Vercel** |
| Itinerary generation | **Claude Haiku** |

## Roadmap

**Hackathon build:**
1. Mentor feedback
2. Build Next.js + Supabase
3. Wire up Claude Haiku
4. Record demo video

**Beyond the hackathon:**
- Real flight/venue disruption data via booking APIs
- Live pricing and availability through maps and booking APIs

---

*NHSY — group trip planning, without the group chat arguments.*
