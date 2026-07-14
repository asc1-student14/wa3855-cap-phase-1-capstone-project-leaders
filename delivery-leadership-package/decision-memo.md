# Decision Memo — _short title here_

> Copy to `delivery-leadership-package/decision-memo.md`. Target length: ~250 words. Write for a non-technical reader. Name the options you **rejected**, not just the one you picked.

**Date:** 7/14/26
**Author:** Shane Sargent
**Decision area:** Day 2 scope tradeoff

## Context

Marketing has requested a new “Compare Plans” link in the navigation menu so they can begin A/B testing. The requested delivery timing is tight, but the project is currently tracking approximately one day ahead of schedule.

Separately, Legal has indicated that customer testimonials require about two weeks for release approval, which creates a risk for including finalized testimonial content in the current delivery. The overall delivery goal remains the same: provide a functional, themed, responsive insurance quote page with a working calculator for the demo.

## Options considered

Option 1: Add Compare Plans during the current sprint if requirements are approved quickly

Pros:

Supports Marketing’s A/B testing request sooner.
Uses available schedule buffer since the project is currently about one day ahead.
May be feasible if the change is limited to a simple navigation link and confirmed target URL.

Cons:

Could introduce risk if the requirement is more complex than expected.
May require additional testing across desktop and mobile navigation.
Could distract from final validation of the core quote experience.

Option 2: Analyze the Compare Plans request now, but defer implementation if it exceeds the available schedule buffer

Pros:

Allows the team to be responsive without automatically increasing delivery risk.
Uses the one-day schedule buffer responsibly.
Protects the original delivery commitment if the new requirement is larger than expected.
Creates a clear decision point based on approved requirements and estimated effort.

Cons:

Marketing may not get the feature in the current sprint.
Some analysis time may be spent on a feature that ultimately gets deferred.

Option 3: Defer Compare Plans immediately to the next sprint

Pros:

Lowest risk to the current delivery.
Keeps the project focused on the originally planned scope.
Avoids late-cycle change management and retesting.

Cons:

Does not take advantage of the current one-day schedule buffer.
Marketing’s A/B testing request is delayed.
May appear less responsive to stakeholder needs.

## Recommendation

Option 2: Analyze the Compare Plans request now, but only implement it in the current sprint if approved requirements confirm it can be completed within the one-day schedule buffer.

Because the project is currently ahead of schedule by approximately one day, it is reasonable to evaluate the new request rather than reject it outright. However, implementation should only proceed if Marketing provides clear approval and final requirements, including the link text, destination, expected behavior, and any tracking or A/B testing needs.

If the requirement can be completed and tested within the available buffer, it may be added to the current sprint. If the effort is expected to take longer than one day, or if requirements are incomplete, the change should be deferred to the next sprint.

## Why

The primary project goal is still to deliver a polished Assembled, running, responsive Evergreen Quote app with the wired quote logic. Since the current schedule has some flexibility, the team can responsibly consider a small scope addition.

However, the available buffer should not be treated as open-ended capacity. A simple navigation link may be low effort, but if the request includes analytics, multiple page variations, styling changes, routing, or new content, the risk increases. In that case, accepting the change could compromise testing and final delivery quality.

This approach balances stakeholder responsiveness with delivery discipline.

## What would change my mind

Compare Plans Decision
The Compare Plans request may be accepted into the current sprint only if all of the following are true:

Marketing provides final approved requirements.
The link destination is confirmed.
No new page build is required.
No complex A/B testing logic is required within the application.
The change can be implemented and tested within one business day.
The original delivery date is not impacted.
If any of these conditions are not met, the request should move to the next sprint.

Testimonials Decision
Due to Legal’s two-week release requirement, the testimonials should be commented out of the current release until approval is received. This avoids publishing unapproved customer statements or using placeholder content that could create confusion.

The recommended approach is to keep the testimonial code in place but commented out so it can be restored quickly once Legal provides approval. At that point, the team can either:

Un-comment the existing testimonial section if Legal approves the current wording, or
Modify the testimonials to meet Legal’s specifications before making them visible.
This approach protects the current delivery from legal/compliance risk while preserving the work already completed and allowing the section to be added back with minimal rework once approval is available.

What Would Change the Recommendation
The recommendation would change if Marketing confirms that the request is limited to a simple navigation link with a final URL and no additional behavior. In that case, the change could likely be implemented and tested within the existing one-day schedule buffer.
