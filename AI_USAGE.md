# AI Usage
### Tools used
Claude (Anthropic) helped with: structuring the audit, writing the reasoning behind each screen, writing the test plan and impact numbers, and building the working prototype from a written spec.

#### Prompts and what came back
* Prompt 1, building the audit: "Map each of the four real user quotes to the exact screen where it happens, and explain why it happens, not just what happens." 

Result: a table matching each pain point to a screen, with a short reason for each. The "current flow" used here was a guess, not the real one, since the brief didn't include it. That was said clearly instead of pretending it was confirmed.
* Prompt 2, building the prototype: A full spec for the six screens, covering layout, accessibility rules, and how it should behave on a slow connection, written like a note to a developer. 

Result: the whole clickable prototype in one go, all six screens, a sidebar explaining each design choice, and accessibility details like button sizes and labels.
* Prompt 3, checking colors: "Give WCAG AA contrast examples for a navy and amber color scheme I can use directly." 

Result: specific colors with contrast numbers, for example, white text on navy scored 6.8:1.

#### Where AI got something wrong, and how it was caught
* Catch 1, a shortcut looked like real behavior. The "type your ID manually" option was set to appear after just one tap of the shutter, not after two real failed photo attempts, since there's no real camera scan happening in a demo. 

Fix: made clear this is a shortcut for the demo, not how the real feature would work
* Catch 2, a guess replaced a reasonable choice. The ID guide first showed a photo on the NIN card image, which is normal for an ID. Trying to make it more accurate, the photo was removed based on a guess that NIN slips don't have photos. That guess was wrong, real NIN slips do have a photo. 

Caught because the person using this deck knew that from experience and said so. A quick search backed them up. 

Fix: put the photo back, based on real information this time, not a guess. 

Why it matters: the fix looked more precise, but it wasn't more correct, swapping one guess for another is easy to miss.

* Catch 3, a button didn't do what it promised. The design said tapping "Continue later" would save your progress and let you leave safely. But in the actual prototype, that button just sent you back to the start screen, like starting over. 

Caught because someone asked directly, "what happens when I click this?" Answering honestly showed the button didn't do what the design said it would. 

Fix: added a short "saved for later" screen that shows before going back to start, so it now matches what was promised. 

Why it matters: this wasn't a wrong fact, it was a case where the feature didn't do what it claimed, easy to miss since the button still worked.







