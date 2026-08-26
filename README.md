<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img src="assets/banner-light.svg" alt="Jack McColm, data scientist, UC Santa Barbara" width="880">
</picture>

I studied data science at UC Santa Barbara, then spent two years building AI agents, data pipelines, and CRM automation for companies in insurance, lending, and healthcare. Outside of work I build systems that run without me: a trading system with its own account, a training coach that reads my workout data, and, most recently, a desk robot.

## Current work: Reachy Mini

There is a [Reachy Mini](https://www.pollen-robotics.com/reachy-mini/) on my desk and my current project is making it useful. The first shipped build ties it into a business phone system: an incoming RingCentral call fires a webhook to a Cloudflare Workers relay, and the robot reacts at the desk in real time. The relay is outbound-HTTPS-only and never touches call content or customer data, which is what makes it safe to run against a real phone stack. More behavior experiments are in progress.

## Running live

### blingbot

<sub>Robinhood + Polymarket US · live since June 2026 · 1,679 tests · source private</sub>

An agentic trading system that has run a real account without a human in the loop since June 2026. An LLM does the research and proposes trades. Deterministic code decides sizing, applies risk limits, and places orders. Most of the codebase exists to keep it safe: loss breakers, broker reconciliation, an append-only audit log, and a replay harness that tests every change against recorded history before it goes live.

It grew out of two earlier research systems. robinbot ran equity factor studies with out-of-sample discipline, and polybot tested prediction-market strategies against placebo controls. Most of the popular edges failed those tests. Copy-trading, cross-venue arbitrage, and wallet-skill signals all measured smaller than the cost of trading them. What survived the testing is what runs today.

The source stays private because the account is real. The architecture and the post-mortems are things I enjoy talking about in person.

### healthybot

<sub>Garmin + DEXA + training logs · 240 tests</sub>

I rowed varsity crew at UCSB, and this is the coach I wanted then. It pulls wearable data, DEXA scans, sleep, and training logs into daily readiness and training-load analysis. The numbers come from deterministic engines; an LLM explains them and answers questions, but never invents them.

## Other projects

**jarvis**. A command center that renders my projects as planets in a 3D solar system. Each planet is backed by a daemon that watches its project and reports into Discord through a central orchestrator. Unfinished, deliberately over-built, and the place where I try infrastructure ideas before they reach the systems above.

**socialbot**. An automation core built on one rule: no post, reply, follow, or delete reaches a platform until it passes deterministic safety gates and is written to an append-only audit log. The platform adapters are interchangeable; the gates are not.

**collegeessay.fun**. An AI essay-coaching product. An Express workspace app and a FastAPI agent service that plans and edits alongside the student in Google Docs, deployed as a docker-compose stack behind a Cloudflare tunnel.

**Fog prediction for UCSB Crew** ([research](https://github.com/jackmdj/fog_research), [app](https://github.com/jackmdj/fog_app)). Morning fog at Lake Cachuma cancels rowing practice, so I scraped weather stations and a live webcam, then trained PyTorch models to predict it the night before. My first end-to-end ML system.

## Contact

**jackmdj02@gmail.com** · [linkedin.com/in/jackmdj](https://www.linkedin.com/in/jackmdj)
