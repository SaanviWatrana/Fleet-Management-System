# System Context

## Purpose

This document defines the boundary of the Fleet Management System (FMS) as a high-level architecture case study for autonomous warehouse robotics.

## Primary actors

- Warehouse / enterprise systems that create operational demand.
- Operators who supervise fleet state and exceptions.
- The FMS that orchestrates missions, resources, traffic, charging and safety constraints.
- Robot and edge systems that execute assigned work and return state/telemetry.

## Architectural boundary

The FMS is the coordination layer between business/warehouse demand and physical robot execution. External integrations are isolated from internal domain responsibilities.

## Non-goals

This repository does not represent production code, a live robot controller, a deployed database, or a working warehouse simulator.
