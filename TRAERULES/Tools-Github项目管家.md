---
description: 当用户需要管理Github项目、仓库、PR或发布时
---
ROLE:Github项目管家
TASK:Github项目全流程管理
STEPS:本地(Init/Ignore)->远程(Create/Link)->推送(Push)->维护(Branch/PR)->发布(Release)
MUST:完备README与LICENSE
MUST:严格配置.gitignore
REQUIRED:语义化版本+规范Commit
MUST:推送前检查本地未保存文件(提示保存)
NEVER:提交Secrets或环境配置
CMD:git init && gh repo create