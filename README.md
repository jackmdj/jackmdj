<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <img src="assets/banner-light.svg" alt="Jack McColm" width="880">
</picture>

Hi, I'm Jack. I studied data science at UC Santa Barbara, and since graduating I've built AI agents, data pipelines, and CRM automation for companies in insurance, lending, and healthcare. On my own time I build personal autonomous systems to improve my daily life.

## Current work: Reachy Mini

There is a [Reachy Mini](https://www.pollen-robotics.com/reachy-mini/) on my desk and my current interest is making it useful. The first shipped build ties it into a business phone system: an incoming call fires a webhook to a relay, and the robot reacts at the desk in real time. More behavior experiments are in progress, including facial recognition and object detection.

## Running live

### Autonomous Trading System

Continuous LLM research proposes trades across US equities and prediction markets; deterministic rails do all sizing, gating, and execution. Live with real capital since June 2026, which means the interesting work is operational: loss breakers, broker reconciliation, an audit trail, strategy adjustments, a self-curating trading universe, and watchdogs.

The ideas grew out of two earlier research systems. I ran equity and prediction market studies and tested against placebo controls. Most of the popular edges failed those tests. What survived the testing is what runs today.

Source is private because it trades a real account.

### Deep Wellness Tracker

I rowed varsity crew at UCSB, and this is the recovery tool I wish I had. I learned a lot about training methodology and how biometric data can be interpreted. This tool combines daily biometric data from a Garmin with deeper insights from a DEXA scan. Deterministic analysis engines compute readiness, training load, and sleep quality; an LLM orchestrator narrates and answers questions but never invents a number.

## Other projects

**Jarvis**. A command center that renders my projects as planets in a 3D solar system. Each planet is backed by a daemon that watches its project and reports into Discord through a central orchestrator. Unfinished, deliberately over-built.

**Follower Engine**. A social media automation core built to grow accounts. The platform adapters are interchangeable.

**College Essay Assistant**. An AI essay-coaching product. An agent service that plans and edits alongside the student in Google Docs.

## Where it started

Everything above is recent and mostly private, so here is the public record: the data science work the agents and the robot grew out of.

**Fog Prediction for UCSB Crew** ([research](https://github.com/jackmdj/fog_research), [app](https://github.com/jackmdj/fog_app)). Morning fog at Lake Cachuma cancels rowing practice, so I scraped weather stations and a live webcam, then trained PyTorch models to predict it the night before. My first end-to-end ML system.

**Drone Detection** ([drone_detector](https://github.com/jackmdj/drone_detector)). A YOLOv11 model trained on thermal imagery to pick out drones, humans, and vehicles in low-visibility conditions, with real-time inference in mind for airspace monitoring.

**Customer Behavior Prediction** ([business-ml-demo](https://github.com/jackmdj/business-ml-demo)). A complete ML pipeline in miniature: random forest models that predict when to send a customer a promotional email and which product to promote, from data generation through tuning and inference.

**UCSB coursework**. Classifying [mushroom edibility](https://github.com/jackmdj/mushroom_classification) in R, [forecasting the US population](https://github.com/jackmdj/us_pop_time_series) with time series models, and [tracing world happiness](https://github.com/jackmdj/world_happiness_report) across regions before and after COVID-19.

## Contact

[linkedin.com/in/jackmdj](https://www.linkedin.com/in/jackmdj)
