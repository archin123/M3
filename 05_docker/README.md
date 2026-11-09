# 05 — Docker

Build and run the software-only M3 demo container. This proves a reproducible container workflow, not a cold-boot Raspberry Pi deployment or physical actuator trigger.

```bash
docker build -t carton-m3-demo .
docker run --rm carton-m3-demo
```

For camera access on Linux, device passthrough and permissions must be configured explicitly. Validate on the target Raspberry Pi before claiming device deployment.
