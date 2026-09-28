# AI Maturity Check for Passenger Airlines

A self-assessment tool that measures how ready a passenger airline is to adopt AI. It is a single HTML file: twenty questions across five dimensions, with a score for each dimension, a radar chart, the two lowest-scoring dimensions, and a maturity profile with a recommended next step.

## How to use

1. Download `AI Maturity Check.html`.
2. Open it in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Answer the 20 questions based on current practice.
4. Review your results.

No installation, server or login is needed.

> **Note:** The radar chart loads Chart.js from a CDN, so an internet connection is required to display it. Without internet, the chart is hidden and the dimension scores are shown as text instead.

## Dimensions

| Dimension | What it covers |
|---|---|
| Data & Systems Foundation | Whether flight, aircraft and passenger data is connected and trusted enough for AI to use |
| Passenger Digital Engagement | How passengers book, change, hear about delays and get through the airport |
| Operations Automation | How crews, turnarounds, flight plans and disruption recovery are run |
| Predictive & AI Deployment | Whether models predict failures, demand and delays, and how AI tools are overseen |
| Organizational Change Capacity | How the airline picks projects, trains staff, checks safety and builds skills |

Each dimension has four questions.

## Scoring

- Each question has five answers, mapped to Stages 1–5:
  1. **Manual**
  2. **Digitized**
  3. **Connected**
  4. **Automated**
  5. **AI-driven**
- Stage 1 represents mostly manual and disconnected work. Stage 5 represents connected, continuously improved practices with advanced automation or AI where appropriate.
- **Dimension score:** average of its four answers (1.00–5.00).
- **Overall score:** average of the five dimension scores.
- **Two lowest dimensions:** always shown as priority areas. Ties are broken in this order: Operations Automation, Data & Systems Foundation, Organizational Change Capacity, Predictive & AI Deployment, Passenger Digital Engagement.

## Maturity profiles

Rules are checked in order; the first one that fits is the result.

| # | Profile | Rule |
|---|---|---|
| 1 | The Early-Stage Operator | Every dimension scores 2.5 or below |
| 2 | The Connected Airline | Every dimension scores 4.0 or higher |
| 3 | The Siloed Airline | Data & Systems Foundation is the lowest dimension, at least 0.75 below every other dimension |
| 4 | The Tools-Without-Traction Airline | Organizational Change Capacity is the lowest dimension, at least 0.75 below every other dimension |
| 5 | The Digitalized-but-Not-Transforming Airline | Passenger Digital Engagement scores 3.5 or higher, and Predictive & AI Deployment scores at least 1.0 lower |
| 6 | Uneven progress | None of the patterns above fit |

## Tech

- Plain HTML, CSS and JavaScript in one file
- [Chart.js](https://www.chartjs.org/) (via CDN) for the radar chart
- Runs entirely in the browser; no data is sent or stored anywhere
