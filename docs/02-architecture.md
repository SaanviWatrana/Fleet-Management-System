# Architecture Decomposition

## Layers

1. **Enterprise / Warehouse Layer** — demand, orders and operational context.
2. **Orchestration Layer** — fleet, mission, traffic, charging, resource and workflow decisions.
3. **Operations Layer** — monitoring, configuration, safety and analytics.
4. **Integration Layer** — adapters and contracts between FMS and external systems.
5. **Robot / Edge Layer** — AGVs, AMRs, PLC interfaces, sensors and telemetry.

## Core principle

The architecture separates *decision ownership* from *physical execution*. The FMS coordinates the fleet; individual vehicles and edge systems execute vehicle-specific behavior.

## Cross-cutting concerns

Safety, observability, configuration and integration affect multiple functional domains and should not be treated as isolated features.
