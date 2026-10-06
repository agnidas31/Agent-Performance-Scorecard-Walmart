# Agent Performance Scorecard (demo)

**Live demo:** https://zorro2018.github.io/Agent-Performance/

A single-file, interactive scorecard that grades contact-center agents month by month on a weighted
composite of quality, productivity and adherence KPIs. It's built for coaching, not policing: every grade
can be traced back to the raw KPI values, the benchmark each one was scored against, and the weight it carries.

> **All data in this demo is synthetic.** People, teams, sites, departments, volumes and KPI values were
> generated from scratch by a seeded script. Nothing is derived from a real organization's data.

## What it shows

- **Composite score (0–100)** from up to 10 weighted KPIs: CSAT, contacts per hour, AHT, shift and break
  conformance, shrinkage, call quality, hold %, refused contacts and transfer %. Missing KPIs (e.g. call quality
  for non-voice agents) drop out and the remaining weights re-normalize.
- **Benchmark interpolation**: each KPI scores 100 at its target, 0 at its floor, linear in between, with
  direction-aware handling for lower-is-better metrics.
- **Personalized AHT**: a contact-volume-weighted benchmark built from each agent's actual channel mix.
- **Two lenses**: org-wide benchmarks versus department-relative benchmarks, side by side, with the tier shift.
- **Four growth-oriented tiers**: Exceeding Target, Meeting Target, Below Target, Improvement Focus, each tied to a
  management action.
- **Fairness gates**: low-volume months, ramp-up months for new hires, support roles and visibility-only feeds
  are shown but not graded.
- **Drill-downs**: filters by month, vertical, sub-LOB, department, channel, site, role, location and tenure;
  tier distributions, a quality-vs-productivity quadrant, tenure radar and heatmap, leaderboards, and per-agent
  KPI detail.
- **Light and dark themes.**

## Run it

Open `index.html` in any modern browser. No server or build step is needed (Tailwind CSS and Chart.js load from
public CDNs).

Built by [Victor Chowdhury](https://www.victorbuildsai.com/).
