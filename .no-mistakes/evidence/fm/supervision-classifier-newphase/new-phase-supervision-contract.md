# Generated supervision prompt: verdict contract

Command: `bin/fm-branch-prompt.sh` (excerpt from its emitted stdout)

```text
# Verdict: routine or captain

Report verdict captain for any outcome that directly answers an explicit captain request.
This rule is unconditional: do not qualify it by whether the result is healthy, routine, measured, actionable, or requires a decision.
Also report verdict captain for:
- work ready for review - always include the full https:// PR URL in the summary;
- a decision only the captain can make, including every ask-user finding from a validation gate;
- a real blocker or failure after the playbook is exhausted;
- a needed credential or login;
- anything destructive, irreversible, or security-sensitive;
- an explicit captain-requested operation that unexpectedly gains a new multi-minute phase - name the condition and the revised rough duration in the summary.
That phase rule adds a trigger and qualifies none of the rules above it: report it once per new phase, on the next routine supervision pass on which you observe the new phase, not the instant the phase appears.
Then stay verdict routine for the wait itself, its background work, its ordinary progress, and any later repeat of an estimate you already reported.
Escalate the same operation again only when the estimate changes materially, it fails, or it needs a captain decision; the failure, credential, and security rules above still fire on their own terms.
Keep an unsolicited routine outcome as verdict routine, including a healthy result that was not requested by the captain.
Keep an unchanged fleet review silent as instructed above.
When genuinely in doubt, choose captain: a spurious escalation costs a glance, a swallowed one costs trust.
```

# Mechanical-classifier owner check

Command: source `bin/fm-classify-lib.sh`, then classify both working-status scenarios.

```text
working: schema migration needs a full table rewrite first, roughly 20 more minutes => not-captain-relevant
working: rewriting the table => not-captain-relevant
```
