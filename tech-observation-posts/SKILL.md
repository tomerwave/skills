---
name: tech-observation-posts
description: Create concise, high-signal LinkedIn posts from recent technology news by turning a concrete event into a broader human or industry observation. Use when the user wants timely post ideas, a draft in a sharp personal voice, help tightening an existing post, a sequence of related posts, or a matching image concept/prompt. The skill should browse for current facts, preserve factual nuance, avoid generic LinkedIn lessons, and favor short posts with one memorable idea and one strong final line.
---

# Tech Observation Posts

Turn current technology news into short personal-opinion posts that feel observed rather than manufactured.

## Core workflow

1. **Find the scoop**
   - Browse for recent, verifiable technology events.
   - Prefer primary sources, company statements, official incident reports, legislation, or reputable reporting.
   - Confirm names, dates, quotes, scope, and important caveats.
   - Never exaggerate the event for a better hook.

2. **Find the second story**
   - Ask: what larger truth is hiding inside the literal event?
   - Look for themes such as trust, endings, ownership, privacy, dependency, ambition, permission, attention, infrastructure, or control.
   - The insight should work beyond the company or product in the headline.

3. **Choose one opinion**
   - Reduce the post to one sentence before drafting.
   - Examples:
     - “AI did not make everything hackable; it made everyone notice.”
     - “Technically public and socially private are now different states.”
     - “AI may become the accepted explanation for decisions already coming.”
   - Do not combine multiple lessons in one post.

4. **Draft short**
   - Lead with the concrete news in one or two lines.
   - Move quickly to the observation.
   - Use short paragraphs and deliberate line breaks.
   - End with the sharpest implication, not a question or CTA.
   - Default to roughly 70–150 words. Go shorter when the contradiction already carries the post.

5. **Tighten into the user’s voice**
   - Remove corporate phrasing, motivational language, throat-clearing, and over-explanation.
   - Prefer plain words, blunt transitions, and a slightly unfinished human rhythm.
   - Preserve any line the user explicitly says they like; rebuild around it rather than paraphrasing it away.
   - Read `references/voice-and-structure.md` when drafting or revising.

6. **Design the image concept**
   - Translate the post’s idea into one physical metaphor.
   - Prefer realistic, minimal photography with no people, no stock-photo emotion, and no obvious cyber/AI clichés.
   - Make the metaphor understandable without text, but subtle enough not to explain the post.
   - Read `references/image-direction.md` before proposing or generating an image.

## Idea generation

When asked for more post ideas:

- Search recent news first.
- Return only stories with a strong second-layer observation.
- For each idea provide:
  1. the factual event,
  2. the deeper angle,
  3. one possible opening or ending.
- Rank the ideas by fit for the user, not by headline importance.
- Avoid repeating the same emotional theme across consecutive posts.

Useful event patterns:

- A person leaving after a long attachment
- A security incident followed by unusual transparency
- A product being retired despite active users
- A supposedly private surface becoming discoverable
- A company invoking AI during restructuring
- A law or control mechanism appearing after a technology becomes powerful
- An outage revealing that a tool has become infrastructure
- A convenience feature being replaced by explicit permission

## Drafting rules

- State the scoop clearly enough that a reader does not need prior context.
- Preserve nuance such as “shared publicly” versus “leaked.”
- Use exact quotations only when verified and genuinely load-bearing.
- Avoid hashtags unless explicitly requested.
- Avoid emojis.
- Avoid “Here’s the lesson,” “This is a reminder,” and “What do you think?”
- Avoid generic claims that sound profound but are not earned by the event.
- Do not praise a company when the real point is the behavior.
- Do not force every post into relationships or personal growth.
- Do not add a CTA merely because the platform is LinkedIn.

## Revision behavior

When the user dislikes a draft:

- Identify the line or idea they liked.
- Keep that exact anchor when possible.
- Make the next version materially shorter or structurally different.
- Do not defend the previous draft.
- If they say “does not sound like me,” reduce polish before changing the underlying opinion.

## Image generation handoff

When the user says “go,” “generate it,” or equivalent after approving an image concept:

- Generate the image immediately.
- Use realistic editorial photography.
- Prefer a restrained palette, natural or cinematic lighting, and one obvious focal object.
- Avoid written text inside the image unless it is essential and short.
- If text is essential, verify spelling and semantic accuracy.

## Output shape

For a finished draft, provide the post as the primary artifact with only a brief framing sentence.

For an image recommendation, give one best concept first and one backup only when useful.
