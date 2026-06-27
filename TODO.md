- [ ] Add Prometheus counter fluxora_sse_subscriber_errors_total with label reason='subscriber_callback_throw' in src/metrics/businessMetrics.ts and update deRegisterBusinessMetrics()
- [ ] Update src/streams/sseEmitter.ts to log structured error (streamId + error name/message) and increment the counter when subscriber callback throws
- [ ] Add test in tests/routes/streams-sse.test.ts: one throwing subscriber + one healthy; assert metric increment and structured log emitted; ensure payload not logged

- [x] Update docs/observability.md to document the new metric

- [ ] Run test suite (npm test) and ensure coverage >=95%



