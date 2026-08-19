---
name: Addition Request
description: Request an addition
title: "[Addition]: "
labels: ["enhancement"]
---
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this addition request.
  - type: textarea
    id: what-to-add
    attributes:
      label: What should we add?
      description: Describe what we should add!
      placeholder: You should add...
    validations:
      required: true
  - type: checkboxes
    id: newestver
    attributes:
      label: I have checked this hasn't been added yet.
      description: Are you sure I've already added this feature?
      options:
        - label: I am sure this has not been added yet.
          required: true
  - type: upload
    id: screenshots
    attributes:
      label: Upload media
      description: If possible, please add screenshots/videos to describe what you want.
    validations:
      required: false
