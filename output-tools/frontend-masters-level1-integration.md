# Frontend Masters — Level 1 Integration

Purpose: use Frontend Masters as an instruction/practice provider while ThirdStreet/Jamal OS owns the learner-state evidence.

## Flow
1. Calendar assigns a specific Frontend Masters course/lesson and links directly to it.
2. Learner completes the assigned lesson/workshop on Frontend Masters.
3. Learner completes `frontend-masters-progress-check.html`.
4. Tool exports a structured JSON artifact.
5. ThirdStreet/Jamal OS classifies the evidence and updates Gaps, Convergence, retest timing, and future scheduling.

## Evidence rules
- Watching/completing a lesson is not mastery by itself.
- `Completed assigned lesson independently` + independently reproduced code/exercise is stronger evidence than course-progress state.
- `Watched/understood but did not reproduce` = conceptual exposure, not mastery.
- `Completed with support/reference` = assisted performance; schedule later independent retrieval.
- `Partially completed`, `Blocked`, and `Stopped at timebox` preserve the exact restart point rather than silently moving the learner forward.
- Exact production failures become Gaps.

## Provider boundary
This Level 1 adapter does not scrape Frontend Masters, call undocumented/private endpoints, copy proprietary course content, or claim access to account telemetry. The learner supplies the direct course/lesson URL and confirms the outcome.

## Minimum artifact fields
provider, course, URL, lesson/section reached, minutes, outcome, produced artifacts, independent reproduction, confidence, learned/can-do statement, exact Gap, support used, exact restart point, timestamp.

## Future Level 2/3
Only add automated telemetry if Frontend Masters provides an authorized integration surface or partnership. Provider-reported completion remains one evidence source rather than the learner model itself.
