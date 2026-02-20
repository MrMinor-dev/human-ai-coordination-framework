# Operational Reporting Framework

**Human-AI Coordination — Building Alignment With an Amnesic Partner**

---

Staying aligned with an agent that forgets everything overnight is a coordination problem, not a technical one. The infrastructure that solves it isn't AI — it's the same stuff that keeps any distributed team aligned: clear state, structured handoffs, async communication, and drift detection.

HAIOS has exactly one domain: Collaboration. Everything else — skills, knowledge management, database, monitoring — belongs to AOS. The single domain focus is deliberate. The only thing that doesn't transfer if the business were sold is the Jordan-Claude working relationship. Everything else is platform infrastructure. The collaboration layer defines how to work together across time and context when one participant forgets everything overnight.

**The coordination layer**

The structured state document is the foundation. Five sections, each with a defined job: what to focus on next, what's in progress, the last 10 sessions, anything urgent, and the operational IDs and stats the agent needs to act. Every session reads that file first and is productive in one message. That only works because the structure is maintained exactly — updated hundreds of times, never ambiguous about what lives where. The structure is the reason, not just the document's existence.

Async coordination runs through Slack. Instructions, task reroutes, and status checks without opening a full session. The agent classifies the message, parses the command, logs receipt, executes, and acknowledges. Neither side needs to be available at the same time.

The handoff contract is the coordination artifact that scales across tools. A schema all 8 production skills use when passing work between phases: what was done, which files changed, current state, errors encountered, what's next. Standardized so any skill can pick up where another left off without asking.

**The reporting layer**

Reporting here doesn't mean dashboards. It means inspection — building visibility into a system that would otherwise be opaque.

Journey capture logs decisions, trade-offs, and failures as they happen, not reconstructed after. 359 sessions of organizational memory — what was tried, what broke, what the fix was, why a different direction wasn't taken. Without it, every session is the first one.

Drift detection runs on the coordination relationship itself. Approval rate above 95%, challenge rate below 5% — that looks like a healthy working relationship. It's rubber-stamping. I built the warning flag in because the number that signals a problem looks identical to the number that signals trust. You have to define which is which in advance, or you won't notice when it shifts. Same pattern as content compliance monitoring: the metric that signals a problem can look identical to the metric that signals health.

Prioritization is explicit in the state document — strategic hierarchy visible at session start, flags with due dates, status by area. Not held in anyone's head. Written down, updated, available to the agent before it makes its first decision of the session.

**Why it matters:** Program coordination at scale is a communication and reporting problem. TPMs spend most of their time keeping distributed stakeholders aligned — scope, changes, who needs to decide. The difference here is one of the stakeholders forgets everything overnight and can't ask for context. Building coordination infrastructure for that constraint is the same skill applied to a harder problem.
