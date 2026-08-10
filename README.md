# Bots — Dirty Dynamics Lab

A deliberately inexpensive, instrumented physics sandbox for developing the small bio-inspired six-limbed service robot.

## Why this exists

The simulator is not intended to make a pretty animated robot. Its job is to cheaply falsify mechanical ideas before hardware: body proportions, joint layout, gait, actuator demand, stability, contact behavior, spring assistance, failure modes, climbing concepts, and eventually sensor/control policies.

The simulated body is also intended to become a teaching environment: controllers can observe body state, attempt actions, receive measurements, and accumulate training/evaluation traces.

## v0.1

- Three.js visualization
- cannon-es rigid-body physics
- six articulated limbs
- motorized hip/knee joints
- gravity, collision, friction, mass and inertia
- live telemetry
- motor kill switch
- variable gait rate
- shove/disturbance test

Run with `npm install` then `npm run dev`.

## Next experiments

1. Replace placeholder geometry with the actual pill-bug body dimensions and mass budget.
2. Model front limbs separately as hand/locomotion limbs.
3. Add joint limits and actuator force/velocity envelopes.
4. Add compliant/spring elements and measure stored/returned energy.
5. Add feet/pads with contact sensing and selectable adhesion models.
6. Record telemetry as machine-readable episodes for controller experiments.
7. Add curl/roll configuration.
8. Add terrain and failure tests (missing limb, weak actuator, low friction, external shove).

The rule: visual fidelity is optional; physically informative behavior is not.
