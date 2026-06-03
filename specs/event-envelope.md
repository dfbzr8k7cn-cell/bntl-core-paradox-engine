# EventEnvelope Contract

The EventEnvelope is the shared data spine for BNTL Core · Paradox Engine.

## Required Fields

- v
- feed_id
- feed_name
- category
- source_type
- ts_iso
- received_at_iso
- source_url
- license
- payload
- normalized_features
- anomaly_score
- confidence
- latency_ms
- quality_score
- freshness_status
- truth_label
- provenance_hash
- last_error
- transform_params
- sample_flag

## Truth Labels

- Live Connected
- Public Endpoint Verified
- EventEnvelope Ready
- Safety Checked
- Sample UI Data
- Unavailable
- Blocked
- Needs API Key
- Error

## Rule

Every app, prototype, connector, export, and validation flow must preserve source context and truth status.