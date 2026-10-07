# GatherWise

A campus event food planner built with AI assistance using Codex.

## Use
Open `index.html` in a browser, or enable GitHub Pages from Settings → Pages → Deploy from a branch → main → /(root) → Save.

Plan an order from RSVPs, turnout, walk-ins, servings per person, buffer, package size, and price. Record actual event attendance and unserved servings to inform later orders. Records are stored only in the current browser; export CSV to keep a copy.

## Calculations
- Expected people = RSVPs × turnout / 100 + walk-ins.
- Target servings = expected people × servings per person × (1 + buffer / 100).
- Packs = target servings / servings per pack, rounded up.
- Cost = packs × price per pack.
- Extra servings = ordered servings minus expected consumption; these are not measured waste.

Example: 50 RSVPs, 80% turnout, 5 walk-ins, 1 serving per person, 10% buffer, packs of 8 at $12 → 45 expected people, 7 packs, 56 servings, $84.

## Research
EPA recommends source reduction, planning, and tracking food waste to guide changes:
- https://www.epa.gov/sustainable-management-food/prevent-wasted-food-through-source-reduction
- https://www.epa.gov/sustainable-management-food/tools-preventing-and-diverting-wasted-food

Example defaults are assumptions, not researched campus averages. Leftovers are not necessarily discarded. No avoided-emissions or proven waste-reduction claim is made. Review dietary requirements separately.

## Verification
Local browser checks: default example, zero-attendance result, rejection of leftovers exceeding ordered servings, leftover percentage, and persistence after reload. No AI calls are made while using the app.

## Assignment handoff
Submit the finalized prompt PDF and this repository link. Include the live GitHub Pages URL once enabled. Review the research personally and retain a genuine, focused refinement request; the assistant-generated specification should not be presented as a student-authored prompt history.
