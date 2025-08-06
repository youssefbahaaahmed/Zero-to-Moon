# Dynamic Bitcoin DCA Strategy

This repository implements a **dynamic Dollar Cost Averaging (DCA)** strategy for Bitcoin, built specifically to compete in the [Hypertrial Stacking Sats Tournament](https://www.hypertrial.ai/stacking-sats).  

## Overview

- **Objective**: Optimize Bitcoin accumulation over rolling 365-day windows by dynamically adjusting purchase percentiles based on historical price signals.  
- **Tournament**: Solutions are evaluated on a daily backtest across all 365-day windows, using the “win‐rate” metric against a uniform-buy benchmark. Top-performing strategies earn leaderboard points in the Stacking Sats challenge.  
- **Key Features**:  
  - Custom signal generation (e.g. log-price z-scores, on-chain metrics)  
  - Parameter fitting via differential evolution or Bayesian optimization  
  - Full reproducibility: uses the template’s mask and metric functions to ensure exact alignment with tournament scoring rules  

## Usage

1. Clone this repo:  
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
