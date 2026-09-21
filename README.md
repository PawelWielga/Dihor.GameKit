# Dihor.GameKit

Home of the Dihor GameKit family: reusable, modular building blocks for game development.

## GameKits

- [Dihor.GameKit.Dice](https://github.com/PawelWielga/Dihor.GameKit.Dice) — framework-agnostic 3D dice rolling with Three.js and cannon-es.
- [Dihor.GameKit.Networking](https://github.com/PawelWielga/Dihor.GameKit.Networking) — transport-neutral multiplayer communication for .NET, TypeScript and Dart consumers.
- [Dihor.GameKit.Board](https://github.com/PawelWielga/Dihor.GameKit.Board) — board and pawn movement primitives, currently in development.
- **Dihor.GameKit.Cards** — planned reusable toolkit for decks, hands, shuffling and common card operations.
- **Dihor.GameKit.Coin** — planned reusable toolkit for coin flips, randomization and visual presentation.

For the family-level priority needed to finish PartyBeam before expanding the kit set, see [docs/partybeam-first-mvp-roadmap.md](docs/partybeam-first-mvp-roadmap.md).

## Landing page

The public landing page lives in `site/` and is deployed to GitHub Pages from `main`.

To preview it locally:

```bash
cd site
python -m http.server 8080
```

Then open `http://localhost:8080`.
