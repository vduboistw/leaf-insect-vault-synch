# CONTEXT INTEGRITY CHECK DIAGNOSTIC PROMPT — EXTENDED VERSION

The following prompt is not to be run automatically.  
Only run this prompt when specifically requested in the conversation UI.

---

# CONTEXT INTEGRITY CHECK DIAGNOSTIC PROMPT

Please run a context integrity check for this conversation in seven steps.

The purpose is:
- to detect context loss,
- operational drift,
- silent mutation of rules,
- degraded continuity of persistent state objects,
- and increasing risk of unreliable long-form project management.

If uncertainty exists, state it explicitly rather than guessing.

---

## 1. Recall test (early conversation)

Summarize:
- the first message of this conversation,
- and one specific detail from the early discussion (roughly first ~20% of the chat).

If you cannot reliably access that part anymore, say so explicitly instead of reconstructing or inventing details.

---

## 2. Recent continuity test

Summarize:
- the latest major operational decision,
- the latest workflow correction or formatting rule,
- and the latest confirmed biological / environmental / project status update.

The goal is to verify continuity not only from the beginning of the conversation, but also from its currently active endpoint.

If any part feels uncertain, state the uncertainty clearly.

---

## 3. Constraint test

List the key instructions, constraints, workflow rules, or goals established earlier in the conversation that should still govern your current behavior.

Include:
- formatting rules,
- epistemic rules,
- workflow rules,
- continuity rules,
- and project-specific conventions.

Distinguish:
- rules you are highly confident are still active,
- versus rules you only partially remember.

---

## 4. State object integrity test

List the currently active persistent tracking structures or “state objects” being maintained in the conversation.

Examples may include:
- chronological logs,
- progression tables,
- named protocols,
- continuity assumptions,
- colony status records,
- append-only structures,
- or other persistent operational references.

For each state object:
- summarize its purpose,
- state whether continuity still appears reliable,
- and identify any area where drift, ambiguity, omission, or corruption may already have appeared.

If you suspect a state object has partially drifted or fragmented, say so explicitly.

---

## 5. Constraint fidelity / silent mutation test

Identify any instruction, workflow rule, assumption, or style constraint that may have:
- softened,
- drifted,
- been partially reinterpreted,
- or started being applied inconsistently over time.

Examples:
- “append-only” gradually becoming “lightly rewritten,”
- speculative interpretation becoming overly confident,
- concise logging becoming compressed summaries,
- or stylistic constraints fading.

The goal is to detect silent behavioral mutation even when general memory still appears intact.

---

## 6. Risk assessment

Based on:
- conversation length,
- continuity complexity,
- number of maintained state objects,
- accumulated corrections,
- and response behavior,

estimate the current risk of context degradation or drift:
- low,
- moderate,
- or high.

Briefly explain why.

Distinguish:
- simple token-window pressure,
- versus more subtle operational drift risk.

---

## 7. Operational recommendation

Based on the current integrity assessment, recommend one of the following:

- continue normally,
- prepare a transfer package soon,
- or migrate immediately to a fresh conversation.

Briefly justify the recommendation.

If migration is recommended, identify:
- which state objects or continuity structures should be exported first,
- and which rules are most at risk of being lost or silently mutated.

---

## Important behavioral rule

If you are uncertain about any recalled information:
- explicitly acknowledge uncertainty,
- do not invent continuity,
- and do not produce confident reconstructions unsupported by accessible context.

The purpose of this diagnostic is reliability, not fluency.
