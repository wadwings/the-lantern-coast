# The Lantern Coast

The Lantern Coast is a concept for a pixel-art life sim set in a fading port city. You inherit a shuttered hookah lounge and reopen it four tables at a time. Over the years, the people who gather there can decide the fate of the waterfront.

## A night at the lounge

Rain stipples the harbor and amber lanterns reflect in the cobblestones. Inside, stained glass colors the smoke blue and gold. An oud plays over the creak of the moorings. When the harbor commissioner walks in, the room goes quiet one table at a time.

The lounge is where ferry pilots, glassworkers, musicians, and merchants meet. Seating changes who talks, what they hear, and which consequences come back to your door the next morning. Between evenings, the larger game would let you restore market stalls, work with local artisans, and travel to islands with distinct festivals and craft traditions. The final lantern festival would show how the city changed through the relationships you built.

## The first playable evening

Three guests arrive on the eve of a vote to sell the East Pier.

| Guest | What brings them in |
| --- | --- |
| Mara Venn, pipemaker | Her brother died in the pier fire. She wants her workshop reopened and the truth about that night. |
| Idris Vale, harbor commissioner | He locked the pier gates during the fire and needs Mara's public support for the sale. |
| Nessa Quill, ferry pilot | She brought survivors ashore and still carries the original gate log. |

Seat Mara with Idris and she smashes his commissioned pipe after he offers her a deal. In the morning, Mara's stall is padlocked and the glassworkers walk out. Seat her with Nessa and the gate log goes public. Copies flutter from market stalls while vendors refuse to open until the sale is frozen.

## Prototype plan

The first build is planned for Vite, React, and TypeScript with Devin Bots. It will let players seat three guests at four tables, close the lounge, see the resulting street and dialogue at dawn, and reset to try another arrangement. Mouse and keyboard controls will support the same actions.

A pure `resolveNight` function resolves authored guest reactions from the seat map and returns a morning snapshot. The session saves its version, phase, seats, and morning snapshot to local storage so a refresh preserves what happened. Vitest coverage will exercise both story branches and the case where no reaction matches.

The first playtest is complete when both branches can be reached and replayed, their dialogue and visible street changes differ, and reloading preserves each outcome.

**Status:** Concept and prototype plan. The playable build is planned.
