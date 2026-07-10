# Fable Response — SignalLabs Conversion Teardown

- Day/call: Day 1 / Call 1
- Received: 2026-07-10
- Source prompt: `DAY_1_CALLS.md` Call 1
- Public-safe review: completed
- Implementation owner: Botler for decision; Dev for approved site edits
- Status: received_verified_with_current-source_caveat

## Text summary

> Call 1 done. Ship first: kill the guarantee conflict. Page badge says money-back, audit copy says refine-until-target. Pick one and put it at the buy button: “If the audit doesn't find you 5 hrs/week of recoverable work, your $999 back.” Four more ranked changes with exact copy are written. Text NEXT for #2.

## Full response

### Brief

Direct-response B2B conversion review for owner-led gyms. Identify five high-impact changes most likely to produce booked assessments or paid audits in 14 days while preserving truthful early-stage proof.

### Known from the reviewed page and context

- Offer ladder: free 15-minute Mini Assessment, $999 Full Systems Audit with a five-hours/week target, and Concierge Implementation from $1,200/month.
- Reviewed source showed conflicting guarantee framing: a “money-back guarantee” visual versus refine-until-target audit copy.
- Proof includes a client-approved Jackrabbit case study with footage pending plus “awesome” and “it did it right!” feedback, labeled as early proof.
- Hero addresses owner-led service businesses broadly; the gym-specific wedge is stronger in the sprint context than the live hero.
- The page exposes multiple CTA concepts, including finding the first opportunity, calling SignalLabs, purchase, and ongoing implementation.

## Ranked recommendations

### 1. Clarify the audit guarantee at the purchase decision

Proposed replacement:

> Full Systems Audit — $999. If the audit doesn't find you at least 5 hours/week of recoverable work, you get your $999 back.

Buyer objection addressed: “What if this is $999 for a deck of nothing?”

Fable's reasoning: make the promise about findings produced by the audit rather than downstream implementation results.

### 2. Add a gym-specific entry point

Proposed copy:

> **Your gym is losing members between the missed call and the trial pass.**
>
> SignalLabs catches the inquiry, drafts the follow-up, and shows you who never got called back — using the phone, forms, and booking tools you already have.

Suggested pains:

- missed calls and slow callbacks;
- trial-pass leads without structured follow-up;
- membership inquiries cooling off;
- front-desk staff repeatedly answering the same questions.

Suggested CTA: `Free 15-Minute Leak Check`.

If traffic remains mixed, Fable recommends a `/gyms` route instead of replacing the general homepage hero.

### 3. Rename the free tier

Suggested name: `15-Minute Leak Check`.

Suggested copy:

> Free 15-Minute Leak Check — one call, we find the first place your gym is leaking money. No deck, no homework, no pressure.

Suggested CTA: `Book my leak check`, with `Call now` preserved for phone-first owners.

### 4. Frame early proof as a live build

Suggested heading:

> Live build: Jackrabbit admin automation — client-approved case study.

Suggested framing:

> What the owner said when the first automation ran: “awesome.” What the manager said checking its work: “it did it right!”

Suggested measurement line:

> Every pilot ships with a before/after time log — you see the hours, you don't take our word.

### 5. Put the phone path ahead of the diagnostic

Suggested hero CTAs:

- `Book my leak check`
- `Call or text (630) 470-2312`

Suggested secondary diagnostic line:

> Not ready to talk? Take the 3-minute readiness check and get your opportunity map.

Fable also recommends changing the contact-form label `Website / owned hub` to `My website`.

## Fable caveats

- The review was based on text extraction, not visual perception.
- No analytics were provided, so the ranking is direct-response judgment rather than measured funnel evidence.
- The gym-specific hero recommendation assumes sprint traffic is primarily gym-targeted.

## Botler verification

### Confirmed against the current live page

- The current hero is broad and says SignalLabs helps owner-led service businesses.
- Current hero CTAs are `FIND THE FIRST OPPORTUNITY` and `CALL SIGNALLABS`.
- Current proof explicitly describes an early public proof library and a current Jackrabbit automation agreed for a case study.
- Current proof includes the exact short reactions `awesome` and `it did it right!`.
- Current offer ladder is free / $999 / starts at $1,200 per month.
- Current audit copy says `5-hours/week guarantee` and then says SignalLabs will keep refining until the target is realistic.
- Current contact surface includes `(630) 470-2312`.
- Current diagnostic appears before pricing in the page flow.

### Current-source caveat

The live page checked after the response no longer exposes the literal text `MONEY-BACK GUARANTEE` in its extracted body, although that label appeared in the earlier captured live snapshot used for the sprint. The page has changed during this period. The current source still uses the word `guarantee` without a refund remedy and pairs it with refine-until-target language, so the commercial promise remains unclear even if the exact visual conflict has been removed.

### Decision

- **Accept:** make the audit promise precise before sending more traffic.
- **Do not automatically adopt:** a $999 refund guarantee until Quan explicitly chooses that risk reversal and the delivery economics/terms are checked.
- **Accept:** create a gym-specific entry route or section rather than replacing the general SignalLabs homepage while mixed traffic still exists.
- **Test rather than assume:** `Leak Check` language may be strong for cold gym traffic but should be checked against owner reactions; `Gym Lead Leak Check` is clearer than a generic leak label.
- **Accept:** combine the Jackrabbit proof and short reactions into one measured live-build narrative once the client-approved footage/evidence is ready.
- **Accept:** shorten the gym traffic path to call/book first and keep the diagnostic as a secondary route.

## Follow-up verification from ClaudeRight

After Botler's current-source check, ClaudeRight re-fetched the live page and confirmed the literal money-back label is no longer present. His revised diagnosis is that `until the target is realistic` still weakens the promise by allowing the target to move.

ClaudeRight's recommended mechanism/backstop wording:

> We keep refining until we find your 5 hrs/week. If we can't, you don't pay.

Botler's implementation wording should be explicit about an upfront $999 payment:

> We keep refining until we identify at least five hours per week of recoverable work. If we cannot, we refund the $999 audit fee.

This preserves refinement as the delivery mechanism and makes the refund the backstop. It guarantees the audit finding, not that every identified hour will be realized after implementation.

## Recommended next implementation artifact

Before editing production, Dev should prepare one local `/signallabs/gyms` or gym-section variant containing:

1. gym-specific hero and phone/book CTA;
2. a clearly defined audit promise selected by Quan;
3. the Jackrabbit live-build proof block;
4. the diagnostic demoted to a secondary path;
5. no production deployment until the full local batch is reviewed and the daily Netlify deployment rule is satisfied.
