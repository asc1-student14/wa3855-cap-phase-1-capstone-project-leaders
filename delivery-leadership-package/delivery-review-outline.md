# Delivery Review — Evergreen Quote

> Copy to `delivery-leadership-package/delivery-review-outline.md`. Five slides OR one page. Target: 5 minutes spoken, then 3 minutes of questions.

## Slide 1 — Delivery goal & did we hit it?

- Goal: Assembled, themed, responsive Evergreen Quote page with a working calculator is on `main` via a reviewed PR and a green CI run.
- Hit? Yes 

## Slide 2 — What shipped

- [Screenshot of assembled Evergreen Quote app on `main`.](https://github.com/asc1-student14/wa3855-cap-phase-1-capstone-project-leaders.git)
- [Link to the merged PR.](https://github.com/asc1-student14/wa3855-cap-phase-1-capstone-project-leaders/pull/8)
- [Link to the green CI run.](https://github.com/asc1-student14/wa3855-cap-phase-1-capstone-project-leaders/actions/runs/29434883060)

## Slide 3 — Two key decisions

- **Decision 1:** Compare Plans Decision: Review and potentially implement the “Compare Plans” nav link only if Marketing provides final approved requirements and it can be completed within the one-day schedule buffer; otherwise, defer it to the next sprint.
- **Decision 2:** Testimonials Decision: Include the testimonials in the release because Legal has approved them, ensuring the content is used exactly as approved or updated only according to Legal’s specifications.
- (Both should be in `decision-memo.md`.)

## Slide 4 — Risks & injects

- Top risk we tracked: _from risk-register.md._
- The project risks delay or reduced quality if the late “Compare Plans” request expands beyond a simple navigation link and consumes more than the available one-day schedule buffer.
- The project risks stakeholder confidence and release readiness if the quote calculator continues producing incorrect premium amounts or the CI failure prevents the team from validating the build.

## Slide 5 — What I'd do differently next round

- Next time, we could define a clearer change intake process upfront, including how late requests like “Compare Plans” will be evaluated, estimated, approved, and either accepted or deferred based on available schedule buffer. We could also identify legal/content approval dependencies earlier so items like testimonials are reviewed before they become a release risk.


## Q&A prep — likely questions

- Q1: Why did we choose to consider the “Compare Plans” request instead of automatically deferring it?
A: Because the project was approximately one day ahead of schedule, it was reasonable to analyze the request. However, we only wanted to include it if Marketing provided final requirements and it could be implemented and tested within that one-day buffer.

- Q2: Why were testimonials allowed to remain in scope?
A: Testimonials were allowed to remain because Legal approved them. The only condition is that the testimonial content must be used exactly as approved or modified only according to Legal’s specifications.
