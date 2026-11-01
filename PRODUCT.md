# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

The primary audience is SC26 Student Research Competition judges and systems and sustainability researchers evaluating the work.

## Product Purpose

Magellan presents and explains research into carbon-aware scheduling for long-running, stateful workloads across geographically distributed sites. It helps evaluators understand the system's mechanism, inspect its measured results, and assess how migration decisions account for execution time, lifecycle carbon, monetary cost, capacity, and migration overhead.

Success means that an evaluator can understand the research contribution, distinguish it from simpler static or centralized scheduling approaches, and inspect the supporting evidence without claims being overstated.

## Positioning

Magellan decentralizes scheduling and destination-capacity arbitration across peer sites. It evaluates whether a running stateful workload should continue, pause, or migrate; balances predicted completion time, lifecycle carbon, and monetary cost; and transfers task state and ownership only after the destination accepts a migration bid.

## Operating Context

The work covers long-running workloads with movable execution state, including LLM fine-tuning, Dendro numerical-relativity workloads, and synthetic benchmarks. Its evaluation uses CloudLab migration experiments, geographically distributed GCP sites, regional carbon traces, measured migration overheads, and capacity and control-plane scaling experiments.

## Capabilities and Constraints

- Evaluates continue, pause, and migrate actions for running workloads.
- Predicts completion time, lifecycle carbon, and monetary cost and scores feasible actions using weighted objectives and a cost cap.
- Accounts for checkpoint, transfer, restore, regional runtime differences, capacity, and thresholds intended to avoid unnecessary migration.
- Uses destination-side arbitration to accept or reject migration bids based on available resources and competing bids.
- Pre-stages datasets and models, transfers checkpoints, restores execution, and transfers task ownership after an accepted migration.
- Presents separate experiments with distinct baselines; reported percentages must remain scoped to their respective experiments.
- Must not invent research evidence, measurements, benchmarks, affiliations, or claims.

## Brand Commitments

Preserve the Magellan name and the attribution to Will Kaminski and Tufts University. Preserve the research-focused voice and the factual framing of Magellan V2 for the SC26 Student Research Competition.

## Evidence on Hand

- `final_poster.pdf`: supplied research poster.
- `core_policy_comparison.png` and `core_policy_comparison.pdf`: policy comparison evidence.
- `utilization_capacity_comparison.png` and `utilization_capacity_comparison.pdf`: capacity-sensitivity evidence.
- `control_plane_scaling.png` and `control_plane_scaling.pdf`: control-plane scaling evidence.
- `scaling_static_vs_magellan.png` and `scaling_static_vs_magellan.pdf`: lifecycle-carbon scaling evidence.
- The existing website copy contains the supplied measurements and experiment qualifications. Future work must preserve those qualifications and must not fabricate additional proof.

## Product Principles

1. Make the decentralized scheduling and migration mechanism understandable before asking the audience to interpret results.
2. Keep performance, carbon, cost, capacity, and migration overhead visible as a multi-objective tradeoff.
3. Tie every quantitative claim to the experiment and baseline that produced it.
4. Make the underlying evidence easy for evaluators to inspect.
5. Preserve scientific precision while explaining the work accessibly to an interdisciplinary research audience.

## Accessibility & Inclusion

The public research website should remain usable with keyboard navigation, semantic structure, meaningful alternative text for figures, responsive layouts, and reduced-motion preferences.
