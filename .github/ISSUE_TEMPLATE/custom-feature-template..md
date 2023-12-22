---
name: New Bug Report 1.4
description: File a bug report
title: "[Feature]: "
labels: ["Feature", "triage"]
projects: ["octo-org/1", "octo-org/44"]
assignees:
  - octocat
body:
  - type: input
    id: contact_details  # Adjusted the id value
    attributes:
      label: Contact Details
      description: What is your name?
      placeholder: ex. Drew
 
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
 
  - type: dropdown
    id: request_type  # Adjusted the id value
    attributes:
      label: Type of request?
      description: Select the type of your request
      options:
        - "New Feature"
        - "Old Feature"
      default: 0
 
  - type: dropdown
    id: os_system  # Adjusted the id value
    attributes:
      label: What is the OS which you want to suggest?
      multiple: true
      options:
        - IOS
        - Color OS
        - Hyper OS
        - MIUI
 
  - type: textarea
    id: suggestion
    attributes:
      label: What are the details of your suggestion?
      description: Explain what do you want 
      render: shell
      value: "Feature details!"
 
---

