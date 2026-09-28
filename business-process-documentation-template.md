## Author note

Use one page for one business action, whether it is implemented by an API, plugin, Flow, or a combination. The page starts at the title below. Add only the steps that exist; include technical details where they affect the outcome. Replace the prompts with verified behavior and remove unused lines. Keep links to the code, registration, Flow, and logs current.

# [Business action]

> **Purpose:** [Who needs this action and why?]
>
> **Complete when:** [What exists or changes when the full process has finished?]

**Starts with:** [Caller and API route, Dataverse event, Flow trigger, or schedule.]

## Example and execution

**Input:** [One representative request, event, or record. Show a sanitized payload only if its fields help explain the action.]

1. **[Component and trigger]:** [What it receives, the important condition, and what it produces. For a plugin, include message/table/stage; for a Flow, include its trigger; for an API, include method/route.]
2. **[Next component, if any]:** [What it receives and creates, changes, or sends onward.]
3. **[Final step, if any]:** [What marks the process as complete.]

**Data crossing a system boundary (if relevant):** [Show one short payload and the destination if a transformation is important to understand.]

**Different outcomes (if relevant):** [Condition → action → result. Include only branches that materially change the outcome.]

## Result and support

**Immediate result:** [What the initiating user/system sees, and when. If it is only an acknowledgement, say so.]

**Verify completion:** [Where to find the final record, file, message, or status and which ID to search for.]

**Failure and replay:** [What can remain after a partial failure, where to find the failed step, and whether rerunning can duplicate effects.]

**References:** [Entry point / contract] · [Code and plugin registration] · [Flow in solution] · [Logs / run history] · [Responsible team]
