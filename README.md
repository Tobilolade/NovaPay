# NovaLend Eligibility & KYC Flow Redesign, README
###### Product Designer (UI/UX) take-home submission for FirstBank Digital Factory.
 What's in this submission:
* Case study deck (PowerPoint): the primary document for the assessment center walkthrough. Audit, all 6 screens with design rationale, accessibility checklist, usability test plan, impact prediction, and AI usage summary.
https://www.figma.com/deck/6ZGdvfbLYRma7U2VkZMPT6/Tobilola-Adebayo_NovaPay-Presentation?node-id=2-108&viewport=-34%2C33%2C0.31&t=dLO7BsgrpxiRpSkA-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1

* Novalend KYC prototype · HTML: Download the HTML File, Open it in any browser; no installation needed.

* Figma link
https://www.figma.com/proto/92f2Teq24jiaDRGUHg75Lr/NOVA_PAY?node-id=6002-1829&viewport=-2669%2C2893%2C0.37&t=TdrSaftXg6hpalQ1-1&scaling=scale-down&content-scaling=fixed&starting-point-node-id=6002%3A1829&page-id=0%3A1

##### How to Navigate the Prototype
* Screen selector (left rail): click any of the six numbered screens to jump straight to it. Each selection also shows a short annotation explaining which pain point or constraint that screen addresses.
* Walk the flow live: starting from Screen 1, tap "Start verification" and proceed through the flow the way a real user would, Continue buttons move forward, the back arrow moves back.
* Language toggle: on Screen 1, tap "Pidgin" to see the instructional copy switch live, this is the localization stretch goal in action, not a static mockup.
* Manual-entry fallback: on Screen 2, tap the shutter to simulate a capture. The first attempt intentionally flags a glare issue so you can see the quality-check and "Use anyway" states; tap the shutter a second time to see the manual-entry fallback appear.
* Error state demo: Screen 4 has a "(Demo: simulate connection drop)" button that jumps to the Error/Retry screen without needing a real dropped connection. From there, "Continue later" shows a brief "Saved for later" confirmation before returning to Start, matching the resumable-draft behavior described in the design rationale.

##### Screen map
* Start / Context, pain points 1 & 4
* ID Capture + manual fallback, pain point 2, hard constraint
* Selfie / Liveness, pain point 3
* Progress system (shown as a persistent element across screens 1 to 4, not a standalone destination)
Confirmation
* Error / Retry (offline state), low-connectivity hard constraint

##### Assumptions made
##### Documented in full in the deck's UX Audit slide, summarized here:

* The current NovaLend KYC flow wasn't provided, so the 8-step flow used for the audit is a reasonable reconstruction based on the four pain-point quotes, not a confirmed reference.
* BVN exists on file but isn't cross-checked before re-requesting ID today, this is the inferred root cause behind pain point 1.
* No manual-entry fallback exists in the current flow at all, rather than existing but being hard to find.

##### Scope note
Per the brief's own guidance that this task is intentionally larger than can be fully built out in the time given, priority went to the six required screens, their rationale, and the required supporting artifacts (accessibility, test plan, impact prediction). Of the three optional stretch goals, a clickable prototype and a localized copy variant (Pidgin, Screen 1) are included; a full trust-signals exploration was scoped out to protect time on the required deliverables.






