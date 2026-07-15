# Go / No-Go — Merge Decision

**Date / time:** Wed 7/15/2026 10:50AM
**Decision:** GO

## Inject Day 3

I’m seeing two active issues that may or may not be related: a reproducible customer-facing quote defect showing an obviously incorrect renters premium of $8,950/month for $25,000 in coverage, and a main CI failure that has been running for the last 32 minutes due to a missing generated asset. I’m asking the team to treat the quote issue as the priority customer-impacting concern while also confirming whether the CI failure is blocking validation or connected to the generated quote behavior. Engineering owns the immediate triage of the premium calculation and reproduction path, while the build/CI owner owns the missing asset investigation; please coordinate findings in the shared incident thread so we avoid duplicate work. I’ll provide communication to stakeholders, including setting expectations with Customer Success and Marketing that we are pausing any new scope decisions until we understand impact, root cause, and the safest next step.

## CI evidence

- My latest run has passed all tests and has successfully pushed through my github actions workflow. link: 'https://github.com/asc1-student14/wa3855-cap-phase-1-capstone-project-leaders/actions/runs/29363607336'
- Workflow file: `.github/workflows/ci.yml`

## What "GO" would mean

What “GO” Would Mean
The Evergreen Insurance project can proceed with the current release because the core delivery goal remains achievable. The project would move forward with the assembled, themed, responsive insurance quote page, including the quote form, navigation, working calculator, and approved testimonials.

Since Legal has approved the testimonials, they can remain visible in the release as long as the content is used exactly as approved or modified only according to Legal’s final guidance.

A GO also means we continue to manage the late Compare Plans request carefully. Because the project is approximately one day ahead of schedule, we can review and potentially implement the request if Marketing provides final approval and clear requirements. However, it should only be included if it can be completed and tested within the one-day buffer. If it takes longer than that, it should be deferred to the next sprint.

A GO does not mean ignoring the reported quote issue or CI failure. It means those items have clear ownership, are being actively triaged, and must be resolved or contained before final delivery.

## What "NO-GO" would mean

A NO-GO decision would mean the project should pause and not proceed to release because there is too much risk to quality, confidence, or delivery stability.

A NO-GO would be appropriate if the quote calculator is still producing clearly incorrect premium results, such as the reported $8,950/month for $25,000 of renters coverage, and the team cannot resolve or explain the issue in time. That type of defect would directly affect the purpose of the demo and could undermine stakeholder confidence.

A NO-GO would also be appropriate if the failing CI run on main is blocking validation, if the missing generated asset prevents the application from building correctly, or if the team cannot confirm whether the CI issue is connected to the quote calculation problem.

The project could also move to NO-GO if the Compare Plans request expands beyond a simple, approved change and threatens the original delivery timeline. Even though we are ahead by about one day, that buffer should be used carefully and should not become open-ended scope expansion.

Because Legal has approved the testimonials, testimonial approval is no longer a reason for NO-GO, provided the approved language is used correctly.

## My call

My decision is GO.

I would proceed because the project can still meet its original training goal: delivering a polished, themed, responsive Evergreen Insurance quote page with a working quote experience. The approved testimonials can remain in scope, which helps the page feel more complete and avoids the need to hide or comment out that section.

The late Compare Plans request should be handled through controlled scope management. Since the project is approximately one day ahead of schedule, I would allow time to review the request if Marketing provides final approval and clear requirements. If it is a simple navigation link with a confirmed destination and minimal testing impact, it may be reasonable to include it. If the request requires more than one day of work, adds complex A/B testing logic, or creates uncertainty, it should be deferred to the next sprint.

The reported quote calculation defect and CI failure are important risks, but they do not automatically change the decision to NO-GO at this point. As a leader, I would make sure the work is routed clearly: Engineering owns the quote calculation investigation, and the CI/build owner owns the missing generated asset issue. The team should determine whether the two issues are related and whether either one blocks final delivery.

My GO decision depends on those issues being resolved, contained, or clearly understood before the final demo/release. If the calculator continues to produce unreasonable quote amounts or the CI failure prevents validation, then the decision should be revisited. But based on the current scope, Legal approval of testimonials, and the available schedule buffer, I would move forward with a GO while maintaining clear escalation points.
