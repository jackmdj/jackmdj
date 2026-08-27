<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img src="assets/banner-light.svg" alt="Jack McColm, data scientist" width="880">
</picture>

Hi, I'm Jack. I studied data science at UC Santa Barbara, and since graduating I've built AI agents, data pipelines, and CRM automation for companies in insurance, lending, and healthcare. On my own time I build autonomous systems and run them for real: one trades my money, one plans my training.

## Current work: Reachy Mini

There is a [Reachy Mini](https://www.pollen-robotics.com/reachy-mini/) on my desk and my current project is making it useful. The first shipped build ties it into a business phone system: an incoming RingCentral call fires a webhook to a Cloudflare Workers relay, and the robot reacts at the desk in real time. The relay is outbound-HTTPS-only and never touches call content or customer data, which is what makes it safe to run against a real phone stack. More behavior experiments are in progress.

## Running live

### blingbot

<sub>Robinhood + Polymarket US · live since June 2026 · 1,679 tests · source private</sub>

Continuous LLM research proposes trades across US equities and CFTC-regulated prediction markets; deterministic, fail-closed rails do all sizing, gating, and execution. Live with real capital since June 2026, which means the interesting work is operational: loss breakers, broker reconciliation, an append-only audit trail, replay-backed strategy changes (nothing ships on vibes), a self-curating trading universe, and watchdogs that survive the host machine literally powering itself off overnight.

It grew out of two earlier research systems. robinbot ran equity factor studies with out-of-sample discipline, and polybot tested prediction-market strategies against placebo controls. Most of the popular edges failed those tests. What survived the testing is what runs today.

Source is private because it trades a real account. I'm happy to walk through the architecture, the post-mortems, and the experiments that didn't survive.

### healthybot

<sub>Garmin + DEXA + training logs · 240 tests</sub>

I rowed varsity crew at UCSB, and this is the coach I wanted then. It turns Garmin wearable data, BodySpec DEXA scans, training logs, and sleep data into daily coaching. Deterministic analysis engines compute readiness, training load, and sleep quality; an LLM orchestrator narrates and answers questions but never invents a number. Same design creed, aimed at my body instead of my portfolio.

## Other projects

**jarvis**. A command center that renders my projects as planets in a 3D solar system. Each planet is backed by a daemon that watches its project and reports into Discord through a central orchestrator. Unfinished, deliberately over-built, and the place where I try infrastructure ideas before they reach the systems above.

**socialbot**. An automation core built on one rule: no post, reply, follow, or delete reaches a platform until it passes deterministic safety gates and is written to an append-only audit log. The platform adapters are interchangeable; the gates are not.

**collegeessay.fun**. An AI essay-coaching product. An Express workspace app and a FastAPI agent service that plans and edits alongside the student in Google Docs, deployed as a docker-compose stack behind a Cloudflare tunnel.

**Fog prediction for UCSB Crew** ([research](https://github.com/jackmdj/fog_research), [app](https://github.com/jackmdj/fog_app)). Morning fog at Lake Cachuma cancels rowing practice, so I scraped weather stations and a live webcam, then trained PyTorch models to predict it the night before. My first end-to-end ML system.

## Contact

**jackmdj02@gmail.com** · [linkedin.com/in/jackmdj](https://www.linkedin.com/in/jackmdj)
