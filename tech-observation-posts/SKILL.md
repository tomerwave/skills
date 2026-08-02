---
name: tech-observation-posts
description: Create concise, opinionated LinkedIn posts from recent technology news, company announcements, incidents, research, or product changes. Use when the user wants to find timely post ideas, connect multiple industry moves into a broader pattern, draft or refine a post in a direct observational voice, choose a visual metaphor, or generate an image concept. Emphasize factual accuracy, a clear second-layer insight, short paragraph rhythm, and understated cinematic imagery rather than generic thought leadership.
---

# Tech Observation Posts

Turn a concrete technology event into a short personal observation with a broader truth underneath.

## Core workflow

1. **Verify the event before framing it.**
   - Search current primary sources whenever the event is recent, disputed, or based on a specific announcement.
   - Prefer the company announcement, official blog, status page, paper, filing, or regulator page.
   - Separate confirmed facts from interpretation.
   - Correct the user's premise gently when needed. Never preserve a stronger hook by overstating the facts.

2. **Find the second story.**
   Ask what the event reveals about one of these deeper tensions:
   - output vs value
   - speed vs maintainability
   - openness vs control
   - transparency vs attention
   - convenience vs ownership
   - capability vs governability
   - detection vs recovery
   - adoption vs infrastructure
   - technically public vs socially private
   - present completion vs future cost

   The event is the evidence. The post is the observation.

3. **Choose one claim only.**
   Do not turn one event into a list of lessons. Reduce the post to one sentence that could serve as its ending. Build only enough context to earn that sentence.

4. **Draft in the user's voice.**
   Read [references/voice.md](references/voice.md).

5. **Refine by subtraction.**
   - Remove generic setup, corporate phrasing, repeated explanation, and forced moralizing.
   - Keep the factual hook explicit enough that a reader understands the scoop without opening a link.
   - Preserve the line or section the user says they like. Revise around it instead of replacing the whole post.

6. **Design the image after the post is stable.**
   Read [references/visuals.md](references/visuals.md).

## Research behavior

Read [references/research.md](references/research.md) when discovering recent stories, validating a specific claim, or connecting multiple announcements.

When proposing post ideas:
- Offer only stories with a real second-layer insight.
- Rank them by strength, not by volume.
- Explain the underlying angle in one or two sentences.
- Avoid generic newsjacking.
- Prefer developments that connect naturally to the user's real expertise in engineering, AI agents, infrastructure, security, observability, governance, and autonomous remediation.

When a story depends on who joined, left, launched, or was absent from an initiative, verify the current state and the launch state separately.

## Draft shape

Use this default structure, but do not force every section:

1. Concrete event or surprising fact.
2. One clarifying sentence that prevents a misleading interpretation.
3. Short adjacent lines or a compact list that sharpens the contrast.
4. Broader observation.
5. A final line that lands without explaining itself.

Keep most posts around 80-180 words. Go shorter when the contradiction is strong enough.

## Paragraph rhythm

The user prefers grouped short lines, not a blank line after every sentence.

Use blank lines to separate ideas, not every line. Adjacent fragments can form a paragraph:

```text
It does not tell us whether:

the product got better
the system became simpler
the code became safer
or the next engineer will understand it six months from now
```

Avoid dense traditional paragraphs, but also avoid the exaggerated LinkedIn style where every sentence floats alone.

## Voice rules

- Be direct, observational, and slightly uncomfortable.
- Sound like a technically informed person noticing a pattern, not a content marketer teaching a lesson.
- Use simple words and short sentences.
- Let the reader make part of the connection.
- Prefer statements over rhetorical questions.
- Use first person sparingly, usually as “I think” or “I wonder” when genuine uncertainty matters.
- Do not add hashtags, engagement questions, calls to action, emojis, or a summary lesson.
- Do not praise brands excessively. Praise a behavior, decision, or pattern.
- Do not make every post about fear. Vary the underlying truth: maturity, trust, economics, ownership, maintenance, attention, or dependency.

## Revision behavior

Interpret feedback precisely:
- “Too long” means remove ideas, not merely compress sentences.
- “Doesn’t sound like me” means reduce polish, abstraction, and explanatory language.
- “More paragraph-like” means group adjacent lines by idea while preserving short sentence rhythm.
- “I like this part” means treat that passage as fixed unless the user explicitly asks to change it.
- “The image is wrong” means re-evaluate the metaphor, not just restyle the same scene.

Offer one best revision first. Provide alternatives only when they express genuinely different angles.

## Image direction

The image should express the deeper idea without illustrating the post literally.

Prefer:
- a physical scene with one clear metaphor
- realistic architectural or documentary photography
- subtle tension rather than drama
- neutral or slightly warm/cool cinematic lighting
- no logos, UI mockups, hacker clichés, robots, floating code, or large text
- no explanatory caption inside the image unless the scene depends on a small natural label

Before generating, describe the metaphor and why it maps to the post. If the user says “go,” generate directly.

## Quality check

Before returning a final draft, confirm:
- The factual hook is accurate and understandable.
- The post contains one central idea.
- The interpretation is clearly an opinion, not disguised fact.
- The ending is earned and not repeated earlier.
- The spacing feels like grouped thoughts rather than one sentence per paragraph.
- The image metaphor matches the whole argument, not one minor detail.
