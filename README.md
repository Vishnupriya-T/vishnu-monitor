# Vishnu Monitor

A real-time infrastructure monitoring dashboard for [vishnuk8s.vercel.app](https://vishnuk8s.vercel.app).

## Features

- **Live endpoint health checks** — polls Home, Blog, About, Gemini API, and RSS every 30 seconds
- **Response time chart** — rolling history of average latency across all endpoints
- **Uptime history bars** — 60-slot visual uptime history with color-coded status
- **Network details** — HTTP status codes, TTFB, CDN region, total bytes transferred
- **Performance scores** — Availability, Performance, and Reliability ring meters
- **Incident detection** — auto-detects high latency, timeouts, HTTP errors, and sustained degradation
- **Remediation suggestions** — each incident includes specific `kubectl`, `vercel`, or `curl` commands to resolve it

## Stack

Pure HTML + CSS + JavaScript (zero build step). Uses [Chart.js](https://www.chartjs.org/) via CDN for the response time chart.

## Deployment

Deployed as a static site on Vercel.
