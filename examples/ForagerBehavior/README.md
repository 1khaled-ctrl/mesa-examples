# Forager Behavior Model

A Mesa simulation demonstrating a modular behavioral framework
for agent-based models.

## Overview

Agents use a **StateMachine** to switch between behavioral states,
and attach reusable **BehaviorModules** for composable logic.

### Agent States
```
searching → (energy low) → resting → (energy restored) → searching
```

### Behavior Modules Used

| Module | Description |
|---|---|
| `EnergyDepletionBehavior` | Drains energy each step |
| `RandomMovementBehavior` | Moves agent to random neighbor |
| `ForageBehavior` | Collects resources from current cell |
| `RestBehavior` | Recovers energy when resting |

Line 1: ## How to Run
Line 2: (empty)
Line 3: ```bash
Line 4: pip install mesa
Line 5: solara run app.py
Line 6: ```
## Purpose

This example is a prototype for the
**GSoC 2026 Behavioral Framework for Agent Models** proposal.

Author: Khaled Saber — github.com/1khaled-ctrl
