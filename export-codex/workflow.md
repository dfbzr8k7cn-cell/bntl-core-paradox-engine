# Export + Codex Workflow

## Purpose

Track how export previews, provenance checks, and Codex-style review entries should move through the BNTL Core system.

## Export Preview Fields

- bundle_id
- created_at_iso
- actor
- mode
- source_count
- truth_label
- included_feeds
- EventEnvelope references
- transform_params
- validation_results
- disclosure_text
- watermark_text
- provenance_hash
- codex_entry_id
- review_status
- sample_flag

## Workflow

Draft → Validation Preview → Provenance Review → Manual Review → Ready for Future Backend

## Rule

A prototype export is not a real sealed record unless a real backend verification system is implemented and reviewed.
