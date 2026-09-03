# Mission & Traffic Design

## Mission lifecycle

`Created → Validated → Queued → Assigned → Dispatched → Executing → Completed`

Exception states can branch into `Blocked`, `Cancelled`, `Failed`, or `Recovery` depending on operational conditions.

## Assignment considerations

At architecture level, assignment can consider:

- Vehicle availability
- Vehicle capability/type
- Current task state
- Battery condition
- Location / estimated travel effort
- Mission priority
- Resource availability
- Safety constraints

## Traffic coordination

Traffic Management owns fleet-level movement coordination. It should reason about shared zones, route conflicts, congestion and priority rather than operating as a vehicle-local navigation algorithm.

## Key interaction

**Mission Management proposes work; Traffic Management validates movement feasibility; Safety can constrain both; the robot/edge layer executes the resulting dispatch.**
