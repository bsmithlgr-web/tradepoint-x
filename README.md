# TRADEPOINT-X Institutional Quant Engine

**Capital preservation. Statistical robustness. Institutional discipline.**

## Overview
TRADEPOINT-X is a production-grade, AI-driven Forex trading system designed for hedge fund launch and SaaS deployment. It integrates regime-aware Bayesian updating, walk-forward validated machine learning, correlation-adjusted Kelly sizing, and multi-layer risk containment.

## Key Features
- **Regime Detection** – Trend/range/volatility classification via EMA/ADX/ATR.
- **Bayesian Engine** – Per-regime Beta posteriors with exponential decay.
- **ML Predictor** – Random Forest with walk-forward CV, purging, embargo, calibration.
- **Advanced Risk** – VaR/CVaR limits, stress testing, tail ratio monitoring, drawdown protection.
- **Correlation-Adjusted Kelly** – Fractional Kelly with parameter uncertainty and correlation penalty.
- **Portfolio Optimization** – Robust Markowitz with 5% max position and Ledoit-Wolf shrinkage.
- **AI Health Monitor** – Stability, calibration error, sensitivity, composite health score.
- **Survival Mode** – Stricter rules for accounts < $1000.
- **Hedge Fund Ready** – NAV calculation, attribution, investor reports, model governance.
- **SaaS Architecture** – FastAPI, multi-tenant, encrypted keys, Redis, PostgreSQL, Docker.

## Installation
1. Clone the repository.
2. Create a `.env` file with your credentials (see `.env.example`).
3. Run `docker-compose up` to start all services.

## Usage
- API documentation: http://localhost:8000/docs
- Trading engine runs automatically via scheduler or can be triggered manually.
- Monitor health and risk metrics via API endpoints.

## Risk Philosophy
"First, survive. Then, thrive." All components are subordinate to capital preservation. The system halts automatically when risk limits are breached.

## License
Proprietary – for authorized use only.
