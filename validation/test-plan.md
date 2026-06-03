# Validation Test Plan

## Unit Tests

- Normalizers and bounds
- EventEnvelope builders
- Truth-label assignment
- Weight cap behavior
- Export preview fields

## Integration Tests

- Connector unavailable behavior
- Stale timestamp handling
- Missing license handling
- EventEnvelope validation
- Export/Codex preview generation
- HUD degraded mode

## Scenario Tests

- Normal payload
- Missing timestamp
- Stale timestamp
- Missing license
- Endpoint unavailable
- High latency
- Malformed payload
- Confidence out of bounds
- Anomaly spike

## Acceptance Rule

No source or module is treated as live until it passes staging, validation, safety review, and provenance review.