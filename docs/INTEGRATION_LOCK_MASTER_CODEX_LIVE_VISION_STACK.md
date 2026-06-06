# Integration Lock — Master Codex + Live Vision Stack

This document is the active integration lock for Paradox Engine + BNTL Core. It integrates the useful architecture from the full conversation and Master Record blocks into the existing app without chopping the system apart.

## Prime Rule

Do not start over. Do not redesign the shell. Do not remove modules. Do not expose private/personal conversation material. Do not turn the app into a wall of random stats.

Preserve the organism. Clean the layers. Make it live and meaningful.

## Public Identity

Public name: Paradox Engine + BNTL Core.
Operator label: Operator / Operator Console.
AI label: Ghost AI / Operator AI.

Do not use MorningStar publicly. Do not use Luna publicly in this version. Do not expose personal emails, family names, children names, grandmother details, private Codex entries, private chat phrases, or personal mythology labels in the public UI.

Private archive concepts may exist only as generic Private Codex / Admin Archive placeholders.

## Locked Template

The existing BNTL-style shell stays locked:

- left rail
- top header / module dock
- central orbital Perception / RealitySignal hub
- right operational rail
- active gates row
- Human Eyes to AI Eyes to Real World strip
- bottom capability / mission / state panels
- bottom operator controls

No panel overlap. No borders crossing text. No mobile horizontal overflow. No giant border overlays. No generic dashboard wall.

## Meaning-First UX

The app leads with one living signal story, not a metrics wall.

The first user experience answers:

1. What changed?
2. Where did it come from?
3. Is it fresh?
4. Is it trusted?
5. What Vision owns it?
6. How does it connect?
7. What should the operator inspect next?
8. What action is allowed or blocked by safety/provenance?

Technical stats stay underneath in drawers, tabs, drilldowns, filters, and detail cards.

## Live Data Rule

No fake running values. Use real public feeds where feasible. If unavailable, show one of:

- NOT CONNECTED
- READY FOR ADAPTER
- NEEDS KEY
- BLOCKED
- STALE
- ERROR
- OFFLINE

If the HUD has a slot, the backend/state layer must provide either real state or a clear unavailable state.

## Live Feed Priorities

- USGS Earthquake GeoJSON -> Seismic Vision
- NOAA SWPC public feeds -> Solar / Geomagnetic Vision where feasible
- NASA EONET -> Natural Events Vision
- Open-Meteo -> Weather Vision
- CoinGecko or accessible crypto endpoint -> Market Pulse if feasible
- Browser/device local status -> Device/System Vision

## Director Responsibilities

The Director links live feeds to the HUD through normalized state.

Director tracks:

- feed registry
- adapters
- refresh intervals
- status: OK / WARN / STALE / ERROR / NEEDS_KEY / BLOCKED / NOT_CONNECTED
- last_ok
- last_attempt
- latency_ms
- freshness_s
- confidence
- source link
- attribution/license
- error message

## Global Connection Chain

Raw source -> Director adapter -> EventEnvelope -> Source Health -> Vision lane -> VISION_STATE -> OS_STATE -> RealitySignal / RJV / Supercell / FRG -> Unified Pulse / What Happened -> HUD modules -> Codex / Export / Provenance.

Nothing should float alone. Every module must either produce state, consume state, explain state, verify state, or preserve state.

## EventEnvelope Contract

Every live or unavailable feed update becomes an EventEnvelope:

- id
- feed_id
- source_name
- category
- vision_id
- timestamp
- status
- freshness_s
- latency_ms
- confidence
- trust_score
- payload_summary
- payload_ref
- source_link
- attribution
- error
- anomaly_score
- operator_next_focus

## VISION_STATE Contract

VISION_STATE includes:

- timestamp
- activeVision
- visions[]
- symbiosisChains[]
- healthSummary
- sourceStatus[]
- devices
- recentEvents[]

Each Vision includes:

- id
- name
- category
- mode
- status
- sourceIds[]
- lastEventIds[]
- trustScore
- freshness
- confidence
- visualPersonality
- connectedAttachments[]
- nextFocus

## OS_STATE Contract

OS_STATE extends VISION_STATE with:

- realitySignal
- stateCore
- rjvSummary
- evolvedSupercells[]
- attachmentStack[]
- agentMode
- codexStatus
- preservationStatus
- sourceList
- eventTimeline
- exportSealStatus
- reviewReadinessMatrix
- workerSync
- sourceHealth
- provenSystemsReforged
- whatHappenedItems[]
- frgRelationships[]
- liveTestRunStatus
- visionModeStack
- cuttlefishProtocol

## Core Systems To Preserve

Do not remove or simplify these systems:

- Perception -> Observe -> Interpret -> Reveal -> Understand -> Action spine
- Vision OS
- Apex Infinite scan / lock / blend
- Director backend orchestration
- Live feed adapters
- RealitySignal
- State Core / OS Core
- RJV / Resonance Junction Vector
- Evolved Supercell
- Attachment Delta
- Attachment Stack
- Symbiosis Graph
- FRG Core / Fusion Relationship Grid
- What Happened / Unified Pulse
- Source Discovery
- Source Health
- Worker Sync
- Live Hooks
- Codex
- Export Seal
- Provenance
- Preservation checks
- Review Readiness Matrix
- Proven Systems Reforged
- Ghost AI / Operator AI
- MONITOR / ENGAGE
- Kill Switch
- Meaningful network artwork
- Human Eyes to AI Eyes to Real World strip
- Live/source/Vision lanes
- Tabs, drawers, filters, search, refresh controls, mobile nav, accessibility states

## Redundancy Merge Without Deletion

What Happened = human explanation and interpretation.
EventTimeline = sequence of events.
Codex = proof/audit record.

Source Health = can we trust this live signal?
Preservation = did we protect the architecture?
Review Readiness = project-set governance.

FRG = relationship grid.
Symbiosis = cross-signal influence.
Proven Systems Reforged = architecture pattern layer.

RealitySignal = heart signal.
State Core = math/interpretation engine.
OS_STATE = full operating state.

## Master Record Integration Map

The old Master Record blocks are private architecture source material and a Vision Mode sourcebook, not raw public UI content.

Useful extracts:

1. Additive-only doctrine: never strip down, never skeleton reset, always layer on, no chopping apart.
2. Vision Mode Library: Clear, Cosmic, Terrestrial, Night, Thermal/IR, Wi-Fi/RF Echo, Aurora, Quantum, Echo Mapping, LiDAR/Spatial Mesh, Signal Fusion, Edge Detection, Motion/Anomaly, Apex Infinite blend, Cuttlefish Protocol.
3. Earth / Space / Signal / Hazard feeds: USGS, NOAA/SWPC, NASA NEO/EONET, Open-Meteo, AQI later, satellites later, device/system status, permission-based network status.
4. Emergency Layer: NORMAL / WARN / CRITICAL safety language.
5. Backend mirrors frontend: HUD slot must map to real state or unavailable state.
6. Signal Command Center: safe Network Health / Device Status / Connectivity Vision / Signal Vision. No unauthorized scanning.
7. Codex / Registry / Glyph logic: immutable log, provenance record, system memory, preservation ledger, export seal history. No private family content in public UI.
8. Experimental seeds: atmospheric/ionospheric public data, particle/physics public data, quantum entropy/signal visualization, replay/forecast overlays. No claims of control and no fake science.

## Vision Mode Stack

Vision modes are living environments, not random filters.

- Clear View: baseline reality/status clarity
- Cosmic Vision: starfield, orbital arcs, solar/geomagnetic bindings
- Terrestrial Vision: terrain grids, seismic/weather/natural event bindings
- Thermal / IR: sensor/feed required; otherwise READY FOR SENSOR
- Wi-Fi / RF Echo: permission-based connectivity status
- Seismic / Ground: quake rings from USGS live feed
- Dream / Probability: replay/forecast drawer, not fake predictions
- Quantum Resonance: entropy/particle visual placeholder; connected only if source exists
- Anomaly Vision: highlights cross-feed anomalies from real state
- Device/System Vision: browser/device/app health
- Experimental Research: public research/source placeholders marked NOT CONNECTED or READY FOR ADAPTER
- Apex Infinite: safe blend of available connected Visions
- Night Vision: visual mode; sensor required for real low-light data
- Edge Detection: camera permission required
- Motion / Anomaly: camera/device permission required
- Signal / Echo: connectivity/system echo status

## Cuttlefish Protocol

Cuttlefish Protocol is the adaptive HUD-skin nervous system. It changes Vision personality based on:

- connected Vision state
- Source Health
- RealitySignal
- Agent Mode
- emergency state
- active attachments

It must not fake data. It only adapts presentation based on real or clearly unavailable state.

## Connected Module Map

- Director feeds Source Health, Vision OS, EventTimeline, What Happened, FRG, RealitySignal, Codex, Export.
- Source Health feeds One Signal Story, What Happened, FRG, Preservation, Review Readiness, and Vision status lights.
- Vision OS feeds active hub, Vision Mode Stack, Apex Infinite, Cuttlefish Protocol, and Attachment Stack.
- RealitySignal feeds the center hub, State Core, RJV, Ghost AI summary, and Agent Mode visual intensity.
- RJV feeds Evolved Supercell, FRG, Anomaly Vision, and What Happened.
- Evolved Supercell feeds FRG, Apex Infinite, Replay/Forecast drawer, and Codex.
- FRG feeds One Signal Story, What Happened, Symbiosis Graph, and next-focus recommendations.
- What Happened feeds EventTimeline, Codex, Ghost AI, and Operator next focus.
- Codex feeds Export Seal, Provenance, Preservation, Review Readiness, and audit history.
- Preservation feeds Kill Switch, Review Readiness, Admin drawer, and update guardrails.
- Attachment Stack feeds Vision Mode Stack, Cuttlefish Protocol, Apex Infinite, and Source Health.
- Worker Sync feeds Source Health, Director health, Review Readiness, and Live Test Runs.
- Live Hooks feed Director and Source Discovery.
- Proven Systems Reforged feeds FRG structure, operator workflow, confidence trail, and Codex audit.

## Live Test Runs

Live Test Runs operate on real feed refresh attempts where possible:

- Start Test Run
- Stop Test Run
- Refresh Live Feeds
- Refresh Source Health
- Run Preservation Check
- Create Export Bundle from current state
- Add Codex Entry from current event
- Toggle MONITOR / ENGAGE

Show reachable feed count, stale/error count, last refresh, pass/warn/fail, and current session ID.

## Final Acceptance

The next working build should show:

- locked template unchanged
- no personal info leakage
- live data where actually connected
- disconnected feeds clearly marked
- one signal story first
- all original modules preserved
- Vision Mode Stack integrated
- Cuttlefish Protocol present
- modules linked through OS_STATE
- no chopping, no dumping, no fake live stats
