---
name: Improvement
about: Fixes, chores, and refactorings; changes to *existing* features. If an improvement
  has lots of steps or changes the public facing API, please use the feature template
  instead.
title: ''
labels: "➕ improvement"
assignees: rrbutani

---

### what

[[ what is this improvement about? here's an example: "Add doc tests for the `AddImm` constructor in `lc3-isa`"
]]

### steps
 - [ ] things

[[ steps to implement this improvement ]]

### where
branch: `imp-`

[[
this should be:
 - N/A if this improvement is not currently being worked on
 - [`imp-<improvement-name>`](tree/imp-improvement-name) if this is being worked on in _this repo_
 - [`org/repo#<branch-name>`](https://github.com/org/repo/tree/branch-name) if this is being worked on in _another repo_

]]

[[
some improvements are closely tied to code that's already in the codebase
i.e.: add a `Display` impl for `PriorityLevel`

for such improvements, it's helpful to link to these bits of code here; we ask that you use permalinks to code in `master` to do so
as an example: [lc3-isa `Word` type](https://github.com/ut-utp/core/blob/4816ece0f2d47e54d989c7a5bc4da9c9f5415f74/isa/src/lib.rs#L82-L83)

see [here](https://help.github.com/en/github/managing-files-in-a-repository/getting-permanent-links-to-files) for details about how to make permalinks on GitHub

for improvements where this isn't applicable, feel free to remove this list
]]
relevant-code:
  - [](https://github.com/ut-utp/core/blob/4816ece0f2d47e54d989c7a5bc4da9c9f5415f74/isa/Cargo.toml#L2)

### open questions

[[ open questions about this improvement ]]
