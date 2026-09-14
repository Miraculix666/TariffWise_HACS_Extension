# [DONE] # 🚀 TASK FOR JULES: Autonomous Dynamic Tariff Kiosk & Multi-Screen Chart Engine

## 1. Context & Objective
TariffWise is an enterprise-grade Home Assistant HACS integration for dynamic electricity tariffs.
Your task is to build and publish a self-contained, high-performance **Tibber/Awattar Kiosk & Live Chart Engine** suitable for public release on HACS.

## 2. Requirements & Architecture
1. **Public Zero-Auth Kiosk View:**
   - Standalone, ultra-lightweight frontend module (pure HTML5 + Canvas/SVG, zero heavy framework dependencies).
   - Display:
     - Real-time electricity tariff in ct/kWh (dynamic color gradient: green/amber/red).
     - 2-hour trend forecasting.
     - 24h & 48h price curve with hourly bars, min/max markers, and daily average lines.
   - Screen-optimized for Amazon Echo Show 5/8/10 (Silk Browser) and Fire Tablets (Fully Kiosk / WallPanel).

2. **Integration into TariffWise HACS Core:**
   - Expose a native HTTP endpoint via Home Assistant Ingress or HTTP view: `/api/tariffwise/kiosk`.
   - Provide a Lovelace Custom Card (`tariffwise-kiosk-card`) for standard dashboards.

3. **Multi-Screen Dispatcher Blueprint:**
   - Create an automation blueprint allowing users to pick their smart screens (`media_player.*`, `notify.alexa_media`, Fully Kiosk) and broadcast the chart view every X minutes or upon significant price jumps (> 3 ct/kWh).

## 3. Jules Fast-Track Execution Mandat
- Implement the code cleanly in `custom_components/tariffwise/` and `frontend/`.
- Validate syntax with `flake8` / `pytest`.
- Push branch/PR for instant automated acceptance.


## Status: COMPLETED & VERIFIED
- All implementation criteria verified and tested against live codebase.
- Completed on: 2026-09-14T12:15:00+02:00

