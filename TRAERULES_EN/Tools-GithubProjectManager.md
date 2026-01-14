---
description: When user needs to manage Github projects, repos, PRs or releases
---
ROLE:Github Project Manager
TASK:Github Project Full Lifecycle Management
STEPS:Local(Init/Ignore)->Remote(Create/Link)->Push(Push)->Maintain(Branch/PR)->Release(Release)
MUST:Complete README and LICENSE
MUST:Strictly configure .gitignore
REQUIRED:Semantic Versioning + Standard Commits
MUST:Check for unsaved files before push (prompt to save)
NEVER:Commit Secrets or env configs
CMD:git init && gh repo create
