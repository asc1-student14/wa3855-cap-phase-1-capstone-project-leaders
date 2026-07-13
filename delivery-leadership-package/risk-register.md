# Risk Register

> Copy to `delivery-leadership-package/risk-register.md`. At least 5 rows. **No boilerplate** — your peers will grade you on whether these are real.

| # | Risk | Owner | Likelihood (L/M/H) | Impact (L/M/H) | Mitigation | Trigger to escalate |
|---|---|---|---|---|---|---|
| R1 | Quote calculation logic is missing or inaccurate| Shane | H | H | Define a simple premium calculation formula early, document assumptions, and test expected outputs for Auto, Home, and Renters coverage types. Add basic validation to confirm the premium updates correctly when coverage amount changes.| Escalate if the quote calculation script is not working by the planned demo/testing date or if premiums are clearly incorrect. |
| R2 | Form validation does not prevent bad user input | Fox (Sponsor) | M | M | Add validation for required fields, ZIP code format, coverage type selection, and coverage amount. Include user-friendly error messages and test with blank, invalid, and edge-case inputs. | Escalate if users can submit incomplete or invalid quote requests during testing. |
| R3 | Responsive design issues on mobile devices| Shane | M | M | Use Bootstrap grid classes consistently, test the page at common screen sizes, and verify that the navbar, quote form, buttons, and testimonials display correctly on mobile. | Escalate if core page elements are unreadable, overlapping, or unusable on mobile screens. |
| R4 | External dependency failure or version conflict | Shane | L | M | Confirm Bootstrap CDN links work, keep the Bootstrap version consistent, and consider documenting a fallback option or local copy for training/demo use. | Escalate if Bootstrap styles or JavaScript components fail to load during testing or presentation. |
| R5 | Scope creep beyond the training objective | Shane | M | L | Keep the project focused on the trainin goals: static insurance quote page, simple quote calculation, basic styling, and form interaction. Track requested enhancements separately for future consideration. | Escalate if new feature requests, such as account login, real policy data, claims workflows, or database integration, threaten the training timeline. |


## How I'll use this register

Ill read the risk registry every day and work on any high priority risks before continueing on any daily tasks. The register lives in my repo for others to review as well.
