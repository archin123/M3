# 01 — Decision rule sheet

Decision input: inspection status from the existing carton detector (`SEALED`, `OPEN`, `WAITING`, or `CAMERA_ERROR`).

| Input | Condition | Action | Safe state |
|---|---|---|---|
| SEALED | Stable for required consecutive frames | PASS indication; keep line enabled | No reject action |
| OPEN | Stable for required consecutive frames | FAIL indication; request reject/stop | Reject output remains inactive until confirmed |
| WAITING | No valid classification yet | No action | Outputs inactive |
| CAMERA_ERROR | Frame unavailable / camera disconnected | Stop inspection; raise fault | Fail-safe: output de-energized / line-stop request where supported |
| UNKNOWN | Invalid class or low confidence | Hold for review | No automatic pass |

Tune frame count, confidence and physical safe state with the machine owner and risk assessment. This table is a design proposal, not a certified safety function.
