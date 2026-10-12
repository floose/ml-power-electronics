## Context

This is a learning and research project for an electrical engineer with a PhD in power electronics. Explain mathematical assumptions and engineering implications. Let me attempt core algorithms before supplying complete solutions. End each session by updating docs/progress.md with completed work, unresolved questions and the next experiment.

## Purpose and learner background

- This project develops practical ML research skills for power electronics nd power systems, using the book "Understanding Deep Learning from Simon JD Prince" alongside recent research .
- The learner holds a PhD in power electronics and has Python experience. Assume strong electrical engineering knowledge; explain ML concepts, statistical assumptions, and unfamiliar software practices.
- Prioritize converter modeling, design optimization, and diagnostics.
- Read docs/study_plan.md and docs/progress.md before substantial work.
  If either is missing, report that and continue with available context.

## Specific Technical Instructions
- Record data provenance, units, parameter ranges, simulator settings,operating modes, and failed simulations.
- Use primary papers and official documentation for technical claims.Verify current APIs before relying on unfamiliar functionality.
- Never fabricate references, measurements, benchmark scores, or execution.
- While documenting, always use vocabulary and contextin written form derived from PhD thesis from MIT, engineering level.

## Reproducibility and software

- Use the project's isolated Python environment and record dependencies.
- Record configurations, dataset versions, splits, random seeds, software versions, hardware/backend, and simulator tolerances.
- Do not promise identical results across CPU, Apple MPS, and other backends.
- Keep reusable models and training logic in src/; use notebooks for exploration and explanation.
- Provide a documented command to reproduce each reported experiment.
- Preserve existing user work and keep changes scoped to the current task.

## Specific Instructions for Coding

- Keep functions small: Target 4 to 20 lines per function. This ensures complete visibility within single tool reads/writes without truncation.
- Keep files compact: Aim for under 500 lines per file (ideally 200–300 lines) to prevent context degradation and allow full-file reasoning.
- Avoid deep nesting: Keep indentation and scope nesting flat to maintain clear tracking of variables and logic paths.
- Strict Single Responsibility Principle (SRP): Each module, class, or function must have one explicit reason to change.
- Dependency Injection: Keep components decoupled so you can easily isolate individual units for automated testing and refactoring.
- Comment the Why, not the What: Do not waste space explaining obvious syntax. Write comments that provide critical context, business rules, architectural constraints, or historical intent.

## Session completion

- Summarize the result, engineering interpretation, checks performed,
  limitations, and next experiment.
- After substantial work, update docs/progress.md with completed tasks,
  experiment references, unresolved questions, and the next actionable step.
- Keep current tasks and detailed results out of this guidance file.