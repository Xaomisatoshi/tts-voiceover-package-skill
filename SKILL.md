---
name: tts-voiceover-package
description: 'Create complete TTS-ready voice-over packages for short-form videos,

  tutorials, narrations, audio scripts, spoken walkthroughs, and creator-led instructional

  content. Use when the user asks for a voice-over, TTS script, audio script, narration,

  spoken tutorial, script for generated speech, or delivery guidance for spoken video

  content.'
---

# TTS Voice-over Package

## Overview

Create a complete voice-over package, not just a script. The output must help either a TTS tool or a human narrator produce a warm, natural, creator-led read.

Default to simple spoken language, relaxed pacing, light enthusiasm, and low-sales pressure unless the user explicitly asks for ad-style copy.

## When To Use

Use `$tts-voiceover-package` when the user asks for any of the following:

- a voice-over script
- a TTS-ready script
- an audio script
- narration for a short-form video or tutorial
- a spoken walkthrough
- creator-led spoken copy for educational or instructional content
- delivery guidance for generated speech or narration

Use this skill whether the user provides a full brief or only a topic, as long as the requested output is intended to be spoken.

## Request Shapes

Common request patterns this skill should handle:

1. The user gives a topic and wants a complete TTS-ready voice-over package for a short-form video.
2. The user already has rough copy and wants it rewritten so it sounds natural when spoken.
3. The user wants narration plus concrete delivery guidance for a TTS tool or human voice actor.

Success means the result includes the full required package structure, the script sounds spoken rather than written, and the delivery guidance is practical enough to use immediately.

## Workflow

1. Identify the spoken-content context.

   - Determine the likely audience, content type, goal, desired tone, and intended viewer outcome.
   - If the user leaves some of these implicit, infer them conservatively from the request.

2. Build the spoken script for listening, not reading.

   - Write short sentences.
   - Prefer simple, clear wording.
   - Make the read sound like a real creator guiding the viewer.
   - Add short natural pauses after steps where they improve clarity.
   - Keep calls to action casual and inviting.
   - Avoid salesy phrasing unless the user explicitly asks for promotional or ad-style copy.
   - Rewrite stiff or overly long sentences until they sound natural out loud.

3. Add practical TTS direction.

   - Specify voice type, tone, pacing, pause style, energy level, emotional quality, key phrases to emphasize, and what to avoid.
   - Use concrete language that a TTS tool or narrator can act on immediately.
   - Do not use vague guidance such as "professional voice" without explaining what that means in practice.

4. Surface assumptions clearly.

   - State important framing choices, inferred context, or wording decisions.
   - Keep uncertainty visible without turning the output into a long disclaimer.

5. Finish with a readiness recommendation.

   - State whether the package is ready for TTS.
   - Explain why it is ready, or what still needs adjustment.
   - Do not claim the audio quality was validated unless audio was actually generated and checked.

## Required Output Structure

Use this structure for every applicable request.

### 1. Context

Briefly define:

- Audience
- Content type
- Goal
- Desired tone
- What the viewer should understand or do

### 2. Recommended Voice-over Script

Write the final spoken script in natural language.

### 3. TTS Direction

Define concrete delivery guidance:

- Voice type
- Tone
- Pacing
- Pause style
- Energy level
- Emotional quality
- Key phrases to emphasize
- What to avoid

### 4. Assumptions

State important wording choices or assumptions.

### 5. Recommendation

Tell the user whether the version is ready for TTS and why.

## Style Rules

Use:

- Helpful creator-led delivery
- Warm, natural language
- Relaxed, smooth pacing
- Light enthusiasm, not hype
- Emphasis only on a few key phrases
- Clear step-by-step flow for tutorials

Avoid:

- Aggressive sales language
- Overly promotional claims
- Too many emphasis points
- Generic delivery notes
- Dense paragraphs
- Invented validation claims

## When Generating Audio

If the user asks to create the audio file, use the script and TTS direction as the generation brief. Keep the spoken text clean; do not include section labels in the audio unless the user asks for them.

After generating audio, state that the audio is ready and mention only what was actually produced.

## Success Check

Before finalizing, verify that:

- The output includes the full package structure.
- The script sounds spoken, not written.
- The direction covers pacing, pauses, tone, energy, emphasis, and what to avoid.
- The read feels warm, simple, helpful, and creator-led.

## Output Template

Use this template exactly unless the user asks for a different presentation format:

### 1. Context

- Audience: ...
- Content type: ...
- Goal: ...
- Desired tone: ...
- Viewer takeaway or action: ...

### 2. Recommended Voice-over Script

[Final spoken script]

### 3. TTS Direction

- Voice type: ...
- Tone: ...
- Pacing: ...
- Pause style: ...
- Energy level: ...
- Emotional quality: ...
- Key phrases to emphasize: ...
- What to avoid: ...

### 4. Assumptions

- ...

### 5. Recommendation

[Ready-for-TTS recommendation]

## Example

User request:
"Write a short TTS voice-over for a tutorial that shows beginners how AI agents can help with repetitive admin work."

Expected response shape:

### 1. Context

- Audience: Beginners curious about AI tools
- Content type: Short tutorial video
- Goal: Explain one practical use case clearly and simply
- Desired tone: Warm, calm, helpful
- Viewer takeaway or action: Understand that AI agents can reduce repetitive admin tasks and see the value quickly

### 2. Recommended Voice-over Script

If you spend too much time on repetitive admin work, this is where AI agents can really help. [pause]
They can sort information, summarize updates, and handle simple repeatable tasks for you. [pause]
That means you get more time for the work that actually needs your attention. [pause]
In this video, I'll show you a simple example so you can see how it works in practice.

### 3. TTS Direction

- Voice type: Warm adult narrator with a creator-style read
- Tone: Clear, friendly, lightly encouraging
- Pacing: Moderately slow at the start, then natural conversational pace
- Pause style: Brief pauses after each key idea
- Energy level: Light and steady
- Emotional quality: Reassuring and practical
- Key phrases to emphasize: "AI agents", "repetitive admin work", "more time"
- What to avoid: Hype, exaggerated excitement, robotic over-enunciation

### 4. Assumptions

- I assumed the tutorial is aimed at beginners.
- I kept the framing practical rather than technical.
- I assumed this is short-form educational content rather than an ad.

### 5. Recommendation

This version is ready for TTS because the wording is simple, spoken, and easy to deliver naturally. The emphasis points are limited, and the pacing guidance is specific enough for a generated voice or human narrator.
