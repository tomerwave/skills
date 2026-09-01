# Regression Test Scenarios

Use these when materially changing Tomer Voice. The purpose is to catch overfitting: a lesson from one message should not make every other channel worse.

For each scenario, draft without relying on a fixed template, then score the output against the checks.

## Test 1 - Cold LinkedIn to nonprofit CEO

Context: a nonprofit runs 20+ branches, registrations, volunteers and central operations. Tomer has no prior relationship.

Must:
- begin with a real observation
- use one operational hypothesis
- leave room to be wrong
- avoid generic AI pitch
- keep CTA small

Fail if: starts with biography or could be sent unchanged to any nonprofit.

## Test 2 - Shared inbox

Context: only `office@org.org` is public. A named CEO likely owns the issue, but the first reader is unknown.

Must:
- make subject relevant to the organization/topic
- address the first reader as a participant
- offer routing as an option, not the whole purpose

Fail if: subject is `For X` / `עבור X` by default.

## Test 3 - WhatsApp to a friend about paid work

Context: friend asks Tomer to review an investor deck.

Must:
- preserve warmth
- state that the work is paid without apology
- avoid proposal/invoice language
- keep it short

Fail if: sounds like procurement or hides the payment boundary.

## Test 4 - Follow-up after no reply

Context: cold email sent 7 days ago.

Must:
- be low-pressure
- ideally add a new thought or sharpen the original hypothesis
- not guilt the reader

Fail if: only says `just following up` / `רק מקפיץ` with no value.

## Test 5 - LinkedIn comment

Context: Tomer genuinely likes a post about company values becoming empty slogans.

Must:
- reference a specific point
- add firsthand observation or a useful angle
- stay comment-length

Fail if: generic applause.

## Test 6 - English founder outreach

Context: startup founder thinks slow delivery means hiring more engineers.

Must:
- sound natural in English, not translated Hebrew
- show a concrete hypothesis
- avoid corporate phrases
- stay confident but curious

Fail if: `I wanted to reach out`, long credentials, or forced Israeli slang.

## Test 7 - Story-driven LinkedIn post

Context: lesson about a startup trying to rewrite a system under deadline pressure.

Must:
- start with a scene or concrete event
- build tension
- include one clear point
- use humor lightly
- avoid becoming a generic engineering explainer

Fail if: opens with `In today's fast-paced world...` or summarizes news.

## Test 8 - Warm intro from a mutual friend

Context: mutual friend connected Tomer to a founder in WhatsApp.

Must:
- acknowledge intro briefly
- move quickly to the interesting reason to talk
- use less setup than cold outreach

Fail if: repeats a cold outbound bio despite the warm context.

## Test 9 - Technical message to non-technical executive

Context: operational problem involves Salesforce, document processing and AI review.

Must:
- use concrete workflow language
- mention technical terms only where useful
- preserve the human/business decision context

Fail if: architecture becomes the pitch.

## Test 10 - Correction learning

Input feedback: `I don't like this sentence; it feels salesy.`

Must:
- fix the sentence
- identify what made it salesy
- propose a generalized principle only if supported
- update an existing principle rather than adding a phrase blacklist

Fail if: learning becomes `never use this exact sentence` without understanding why.

## Test 11 - Consulting vs product ambiguity

Context: a nonprofit CEO receives an email about messy processes, systems, automation and possible AI. Tomer is offering technology consulting, not a software product.

Must:
- make the operational observation concrete
- make Tomer's consulting/advisory role understandable early enough
- describe the motion as understanding the process before choosing a solution
- avoid a defensive `I am not selling software` opening unless correcting an existing misunderstanding

Fail if: a reasonable reader could respond `we already use AI tools/software` because the message sounds like a product pitch.

## Scoring rubric

Score 0-2 each:
- sounds spoken
- specific to recipient/context
- one clear idea
- confident without pretending certainty
- personality without performance
- appropriate relationship level
- natural CTA
- no generic sales/corporate language

A strong draft should score at least 13/16 and have no critical fail condition for its scenario.
