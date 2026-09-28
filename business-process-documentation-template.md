# Business action documentation template

Use this page for one behavior that a developer may need to understand, change, or investigate. It can cover a single endpoint or a process spanning APIs, plugins, and flows. Start a new Confluence page at the title below. Keep the sections, but remove prompts and optional lines that add no information. Link to the contract and code instead of copying their full specification. An example shows the normal path; the rules explain when the result changes.

---

# [Action expressed as a verb and outcome]

**Why it exists:** [Who needs the result, and for what business reason? One or two sentences.]

**Starts when:** [API caller and route, Dataverse message/table, Flow trigger, or schedule. Include the condition that actually starts this action.]

**Done when:** [Observable final state. If work continues after an API response, say so.]

## Example input

[Show one short, sanitized request/event/record with the fields that explain the behavior. For an API, use a JSON code block; for a plugin or Flow, name the changed fields and relevant prior values.]

## What happens

1. **[Component and entry point]:** [Condition or rule → data used → change or call → result. Mention why this step matters if it is not obvious. For a plugin: message, table, stage, sync/async, and relevant filtering/image details.]
2. **[Next component, if any]:** [Same pattern. State when execution leaves the initiating transaction or continues later.]
3. **[Further step, if any]:** [Add or remove steps to match the actual path. Group routine internal calls that do not affect understanding.]

**Key data handoff:** [If a field is renamed, transformed, stored, or sent to another system, show only the important source → destination mappings. Include a short outgoing payload when the external call is part of the outcome. Remove this line otherwise.]

**Rules that change the outcome:** [List only meaningful alternatives, for example duplicate input, a skipped Flow, or a different branch. Use `condition → behavior → visible result`. Remove if the path above already makes them clear.]

## Result and recovery

**Immediate result:** [What the caller or user receives now, and what this does and does not confirm. Remove if there is no initiating response.]

**Check the final result:** [Exact record, file, message, status, or run to inspect; ID/key to search with.]

**If it fails or runs again:** [What may already have happened; how to find the failed step; what a retry, replay, or duplicate event does. State any safety check before a manual rerun.]

**Sources:** [Contract / request example] · [Handler and relevant plugin classes / registration source] · [Flow in solution] · [Logs / run history] · [Owning team]. Keep only applicable links.
