# Dispatch resolver context package, live transcript (2026-09-23)
Briefs scaffolded by the real bin/fm-brief.sh in an isolated FM_HOME; resolver run unmodified with a placeholder key against https://api.typesafe.ai (real 401).
A recording curl saved the POST body and forwarded it to /usr/bin/curl unchanged.

Scaffolded ship brief size:    13451 bytes; scout brief:     7274 bytes

## port-task_brief.md resolver output
dispatch-resolve:
  status: error
  reason: http 401 after 255 ms: {"detail":{"error_type":"authentication_error","message":"Cannot authenticate with the server. Please check your API key and try again."}}
## port-task_brief.md state.task.brief sent to Jev (360 bytes)
~~~~
## Captain's intent
Port the macOS-only screen capture helper to Windows and add a Windows installer. This is a straightforward port of existing behavior.

## Firstmate spec
Follow the existing helper layout.

````text
example config:
```
## Not a heading, inside a fence
```
````

Never delete user captures. Never ship unsigned installers.
SPEC-TAIL-MARKER

~~~~

## scout-task_brief.md resolver output
dispatch-resolve:
  status: error
  reason: http 401 after 188 ms: {"detail":{"error_type":"authentication_error","message":"Cannot authenticate with the server. Please check your API key and try again."}}
## scout-task_brief.md state.task.brief sent to Jev (169 bytes)
~~~~
Brief kind: scout (report only)

## Captain's intent
The pager export is slow, find out why.

## Firstmate spec
Profile the export path and report the top three costs.

~~~~

## freeform.md resolver output
dispatch-resolve:
  status: error
  reason: http 401 after 207 ms: {"detail":{"error_type":"authentication_error","message":"Cannot authenticate with the server. Please check your API key and try again."}}
## freeform.md state.task.brief sent to Jev (77 bytes)
~~~~
Fix the typo "recieve" in README.md line 12.

No headings here, just prose.

~~~~

## min_confidence 1.5 rejected before any network call
error: malformed rules file: /var/folders/4n/_bv20k5d26dgrq1t5y4l69940000gn/T/tmp.yun1sosAWo/home/config/crew-dispatch.json - min_confidence must be a number from 0 through 1 when present
(recording curl body file absent: no request made)
