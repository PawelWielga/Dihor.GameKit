# Dihor.GameKit family roadmap for PartyBeam First MVP

## Purpose

This document records which GameKits are actually required to finish the first PartyBeam ecosystem MVP and prevents unrelated GameKit expansion from becoming part of the critical path.

Status snapshot: 2026-09-21.

## Required kit set

| Kit | PartyBeam First MVP role | Status |
| --- | --- | --- |
| `Dihor.GameKit.Networking` | communication, discovery, reconnect, timing | required and already integrated |
| `Dihor.GameKit.Board` | Grimcellar board/topology/movement/presentation helpers | required and already consumed |
| `Dihor.GameKit.Dice` | Grimcellar 2d6 combat/presentation | required and already consumed |
| future Cards kit | none | post-MVP |
| future Coin kit | none | post-MVP |

## Ordered family-level priorities

### GK-MVP-01 - protect the Networking integration

PartyBeam must keep using Dihor.GameKit.Networking rather than creating a parallel stack.

Only concrete generic defects discovered by PartyBeam/Reflex/Grimcellar E2E should interrupt the ecosystem critical path.

### GK-MVP-02 - prove Board through Grimcellar

Keep the approved Board prerelease pinned and prove its required workload through the official Grimcellar package on PC/laptop and Android TV.

Only release another Board prerelease if real validation finds a blocking generic defect.

### GK-MVP-03 - prove Dice through Grimcellar

Keep the approved Dice prerelease pinned and prove real 2d6 authoritative combat through the official Grimcellar package.

Cut a new prerelease only if the required runtime path needs fixes that are not present in the currently consumed package.

### GK-MVP-04 - finish PartyBeam ecosystem validation before expanding kit count

Do not make Cards, Coin or another new GameKit a prerequisite for the first PartyBeam ecosystem MVP.

New kits may be designed later, but the MVP milestone should first prove that:

- Networking works under Reflex/Grimcellar real sessions;
- Board works in Grimcellar;
- Dice works in Grimcellar;
- package/release/version pinning across repositories is reproducible.

## Family First MVP completion

The GameKit family has fulfilled its PartyBeam First MVP role when:

- no required PartyBeam E2E scenario is blocked by a generic kit defect;
- all three required kits are consumed as packaged/versioned dependencies rather than copied code;
- any blocking fixes have durable prereleases and downstream pins;
- the PartyBeam ecosystem First MVP is closed.

After that point, broader GameKit roadmap work can proceed independently.

## Per-repository detail

See:

- `Dihor.GameKit.Networking/docs/partybeam-first-mvp-roadmap.md`
- `Dihor.GameKit.Board/docs/partybeam-first-mvp-roadmap.md`
- `Dihor.GameKit.Dice/docs/partybeam-first-mvp-roadmap.md`

The master ecosystem order lives in `PartyBeam.Platform/docs/ecosystem-first-mvp-execution.md`.
