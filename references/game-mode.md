# Game Mode

Use this framework for commercial games, narrative games, prototypes, interactive fiction, live-service systems, and reference-title analysis. Treat player decisions and feedback as the center of the teardown.

## Analysis Framework

### 1. Experience Thesis

- State the player fantasy or emotional promise.
- Define what the player repeatedly does to produce that feeling.
- Distinguish authored atmosphere from playable agency.

### 2. Audience and Play Context

- Identify intended players, session length, platform, input context, and tolerance for complexity.
- Name the expectation set by genre, store page, first five minutes, or comparable titles.

### 3. Core Decision Loop

Model the loop as:

`Situation -> Information -> Decision -> Action -> Feedback -> Consequence -> New situation`

Check whether the player receives enough information to form intent, whether choices change state, and why the loop remains interesting after repetition.

### 4. Verbs, Resources, and State

- List player verbs and the resources they consume or produce.
- Identify visible and hidden state, thresholds, timers, relationships, inventory, and progression gates.
- Find dominant strategies, fake choices, reversible versus irreversible decisions, and failure recovery.

### 5. Narrative-System Coupling

- Map story beats to player action, state change, consequence, and later recall.
- For text-heavy systems, trace `read -> notice -> interpret -> choose -> consequence`.
- Flag emotion that exists only in prose or presentation but has no mechanical expression.
- Preserve the project's accepted narrative baseline; do not silently promote exploratory ideas into canon.

### 6. Pacing and Structure

- Examine onboarding, escalation, chapter or run rhythm, downtime, climax, and ending conditions.
- Identify where novelty enters and how the game avoids content or cognitive fatigue.

### 7. Readability, Fairness, and Feedback

- Check signposting, control clarity, consequence legibility, save/retry behavior, and accessibility.
- Separate intentional uncertainty from missing information.
- Judge whether failure teaches, punishes, delays, or merely repeats content.

### 8. Progression and Return Drivers

- Analyze mastery, discovery, collection, narrative curiosity, social pressure, streaks, and meta-progression.
- Do not label compulsion as retention quality; include the cost to pacing, trust, and theme.

### 9. Presentation as System

- Identify how camera, layout, sound, animation, timing, and input feedback carry information.
- Distinguish production polish from structural clarity.
- Name which effects are functional, atmospheric, or replaceable.

### 10. Production Reality

Estimate relative burden rather than invented schedules:

- content volume and branching multiplication
- art, animation, audio, localization, and accessibility load
- runtime/state complexity and save compatibility
- QA surface, edge cases, and replay testing
- dependence on custom assets versus code placeholders

### 11. Market and Business Fit

When relevant, inspect positioning, audience promise, demo value, streamer/readability value, pricing, DLC or live-service assumptions, and discoverability. Do not force SaaS growth concepts onto a finite premium game.

### 12. Weaknesses and Transferable DNA

- Name the three most consequential design or production risks.
- Identify the smallest mechanism that produces the reference title's value.
- For the user's project, classify each candidate as `保留`, `改造`, or `不采用`.
- Prefer a bounded prototype or chapter slice over a project-wide redesign.

## Game Verdict

End by answering:

1. What does the player actually learn to do?
2. Which loop produces the promised feeling?
3. Where do agency, pacing, or production cost break down?
4. Which mechanism is worth testing in the user's current project?
