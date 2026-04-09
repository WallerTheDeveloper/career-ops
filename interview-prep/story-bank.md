# Story Bank — Master STAR+R Stories

This file accumulates your best interview stories over time. Each evaluation (Block F) adds new stories here. Instead of memorizing 100 answers, maintain 5-10 deep stories that you can bend to answer almost any behavioral question.

## How it works

1. Every time `/career-ops oferta` generates Block F (Interview Plan), new STAR+R stories get appended here
2. Before your next interview, review this file — your stories are already organized by theme
3. The "Big Three" questions can be answered with stories from this bank:
   - "Tell me about yourself" → combine 2-3 stories into a narrative
   - "Tell me about your most impactful project" → pick your highest-impact story
   - "Tell me about a conflict you resolved" → find a story with a Reflection

## Stories

<!-- Stories will be added here as you evaluate offers -->
<!-- Format:
### [Theme] Story Title
**Source:** Report #NNN — Company — Role
**S (Situation):** ...
**T (Task):** ...
**A (Action):** ...
**R (Result):** ...
**Reflection:** What I learned / what I'd do differently
**Best for questions about:** [list of question types this story answers]
-->

### [Performance] Diagnosing frame drops in production AR apps
**Source:** Report #001 — JetBrains — GameDev Solutions Architect
**S:** 3 AR apps at ZAUBAR had frame drop issues in production with no baseline profiling in place.
**T:** Diagnose root causes and restore runtime stability without disrupting ongoing releases.
**A:** Used Unity Profiler and Android Logcat to trace draw call spikes; isolated culprit to overdraw in transparency render stack.
**R:** Eliminated frame drops across all 3 apps, improving runtime stability measurably.
**Reflection:** Establish profiling baselines at project start, not post-release. A performance budget on day one saves a debugging sprint at week twelve.
**Best for questions about:** debugging, performance optimization, production stability, profiling methodology

### [Architecture] Extending a shared AR SDK without breaking downstream projects
**Source:** Report #001 — JetBrains — GameDev Solutions Architect
**S:** Internal teams at ZAUBAR couldn't ship new AR features fast enough — bottlenecked on SDK updates.
**T:** Extend the internal AR SDK with new AR Foundation / ARKit / ARCore features while maintaining backward compatibility.
**A:** Added 3 new AR feature modules with clear interfaces and tests; documented the integration contract for downstream teams.
**R:** Downstream projects onboarded new features the same week without blockers or breaking changes.
**Reflection:** SDK ownership is about contracts, not just code. Interfaces and documentation matter more than internals — that's what enables independent parallel work.
**Best for questions about:** SDK design, API ownership, cross-team collaboration, technical leadership

### [Delivery] Building CI/CD from scratch for multi-platform AR releases
**Source:** Report #001 — JetBrains — GameDev Solutions Architect
**S:** Each AR build required manual QA setup — slow, error-prone, impossible to scale across 4 active projects.
**T:** Automate the build and distribution pipeline for iOS and Android across all active releases.
**A:** Built Jenkins pipeline with signing automation + Firebase App Distribution for both platforms.
**R:** Release cycle dropped from days to hours across 4 projects; removed the human bottleneck from every build.
**Reflection:** Would have added automated screenshot regression testing earlier. CI infra pays back in compound interest — every release you skip debugging is future velocity.
**Best for questions about:** CI/CD, DevOps, automation, release management, cross-platform delivery
