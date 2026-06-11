# Dynamic Trust Scorer for NS-3

A lightweight trust evaluation framework designed for NS-3 simulations.

The Dynamic Trust Scorer continuously monitors packet behavior between communicating nodes and dynamically updates trust scores using behavioral analysis. The framework employs sliding-window monitoring, baseline learning, exponential penalties for repeated violations, and gradual recovery during normal operation.

## Features

- Session-based trust evaluation
- Sliding-window packet monitoring
- Baseline traffic learning
- Dynamic trust computation
- Exponential trust degradation
- Linear trust recovery
- Threshold-based session blocking
- Traffic generation for trust evaluation
- Lightweight and simulation-friendly design

## Architecture

The framework consists of:

1. Packet Observation Layer
2. Sliding Window Monitor
3. Baseline Learning Engine
4. Deviation Computation Module
5. Dynamic Trust Evaluation Engine
6. Threshold Enforcement Module

## Trust Model

### Violation Penalty

Penalty(n) = α × 2^(n−1)

### Trust Reduction

T(new) = T(old) − α × 2^(n−1)

### Trust Recovery

T(new) = T(old) + β

### Blocking Condition

Trust < Threshold

## Documentation

Project documentation is available through GitHub Pages:

```text
https://muthuvenkatesh-24.github.io/dynamic-trust-scorer-docs/
