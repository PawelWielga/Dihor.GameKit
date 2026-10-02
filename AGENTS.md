# AGENTS.md

## Repository role

This repository is the landing/discovery/documentation home for the independent Dihor.GameKit family.

## Family boundary

Dihor GameKits are reusable beyond PartyBeam.

- Networking owns generic communication.
- Board owns generic board/topology/movement capabilities.
- Dice owns generic dice/physics/presentation capabilities.
- Future kits require a coherent reusable responsibility.

`PartyBeam.GameSdk` is not a Dihor GameKit. It is a separate PartyBeam-specific contract/tooling repository.

Do not describe PartyBeam as the owner of Dihor APIs. PartyBeam may drive real-world requirements, but reusable changes must remain useful and correctly named outside PartyBeam.

## Documentation

Keep the landing page and README aligned with actual released/planned GameKits. Do not advertise speculative libraries as available.

## Dependencies/licensing

Family guidance continues to prefer permissive licenses and no paid commercial runtime dependencies.
