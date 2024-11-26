---
name: Bug report
about: Create a report to help us improve
title: ''
labels: ''
assignees: ''

---

name: Bug Report
description: Use this to report bugs.
title: "[Bug]: "
labels: ["bug"]
body:
  - type: input
    id: title
    attributes:
      label: Bug Title
      description: Provide a short and descriptive title for the bug.
      placeholder: Short Description Here
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: What happened?
      description: Describe what happened and what you expected to happen.
      placeholder: Provide details about the issue here.
    validations:
      required: true

  - type: dropdown
    id: platform
    attributes:
      label: Platform & Operating System
      description: Select the platform on which the issue occurred.
      options:
        - Linux ARM64
        - macOS
        - Windows
        - Other

  - type: input
    id: browser
    attributes:
      label: Browser Version
      description: Specify the browser and its version (if GUI-related).
      placeholder: e.g., Safari 17.3.1
    validations:
      required: false

  - type: textarea
    id: logs
    attributes:
      label: Anything Else to add?
      description: Paste any relevant information here.
      render: shell
      placeholder: Paste any relevant info here.
