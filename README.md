# EAMS - Exhaled Ammonia Monitoring System

A handheld breath analyzer prototype that measures exhaled ammonia to support early kidney-health screening in low-resource and rural clinics.

**Screening support, not diagnosis.** This is a research prototype. It does not diagnose kidney disease, and a "Lower Risk" result does not rule it out. No clinical accuracy is claimed. Any accuracy numbers in the project deck come from published literature, not from this team's device. Any model in this repo trained on public or simulated data must be labeled that way.

## Planned architecture (provisional)

ESP32 + gas/environment sensors -> WiFi -> Firebase -> Python API (risk model) -> Flutter app

Sensor choice (MQ-135/DHT22 vs MQ-137/BME688) is still open. Keep code sensor-neutral where possible.

Risk output: Lower Risk / Further Assessment / Higher Risk, with a confidence threshold.

## Repo layout

| Folder | Purpose |
|---|---|
| `firmware/` | ESP32 code: sensor reading, calibration, upload |
| `backend/` | Python API, Firebase integration |
| `ml/` | Data cleaning, feature selection, training, evaluation |
| `app/` | Flutter app |
| `data/` | Dataset notes and small samples. No raw sensitive data in git |
| `docs/` | Design notes, safety/FMEA, dataset audit |

## Getting started

Read [CONTRIBUTING.md](CONTRIBUTING.md) for the branch workflow.

## Status

Scoping. No real breath data collected yet.