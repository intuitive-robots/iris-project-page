# Meta Quest 3 Development Guide

Design XR interactions that feel natural on the Meta Quest 3 by focusing on comfort, clarity, and responsiveness.

## Interaction Principles

- **Hands-first**: Prioritize hand tracking and pinch gestures; controllers are secondary.
- **Clear affordances**: Use sizing, color, and subtle animation to show what can be grabbed or pushed.
- **Short sessions**: Keep each flow under 15 minutes to avoid fatigue.

## Input Patterns

| Scenario | Recommendation |
|----------|----------------|
| Selection | Use ray pointer with confirmation haptics as fallback for hand tracking. |
| Manipulation | Rely on two-handed scaling gizmos with position constraints. |
| System actions | Implement palm-up menu; include voice shortcuts for expert users. |

## Performance Targets

- 90 FPS sustained with ASW disabled.
- GPU frame time under 8 ms and CPU frame time under 10 ms.
- Memory footprint under 2.5 GB.

## Testing Checklist

- Verify guardian boundary prompts appear correctly.
- Validate mixed reality capture composition with standard lighting.
- Test both color passthrough and fully immersive modes.

Document usability findings in the shared IRIS testing template after each playtest.
