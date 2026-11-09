# 04 — Actuator fires

This folder contains a dry-run actuator simulator only. It prints PASS/REJECT/FAIL-SAFE events and does not access GPIO pins or switch a relay.

For a real actuator demonstration, use an appropriately rated isolated driver, a documented wiring diagram, an emergency stop, and a reviewed fail-safe design. Do not connect a Raspberry Pi GPIO directly to mains or a motor.
