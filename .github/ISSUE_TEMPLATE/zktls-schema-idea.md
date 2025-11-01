---
name: zkTLS Schema Idea
about: Propose a new zkTLS verification schema
title: '[schema] <Short Description>'
labels: schema-idea
assignees: ''
---

### Goal / What to Verify
e.g., Prove ownership of Apple devices, as anti-sybil signal

### How to Implement
e.g., Capture GET request to devices endpoint, notarize `/devices` JSON field

### Network Request (Optional)
- **Visit this URL**: e.g., https://account.apple.com/account/manage/section/devices
- **Request this URL**: e.g., https://appleid.apple.com/account/manage/security/devices
- **Method**: GET
- **Relevant Response Snippet**:
  ```json
  ...
  "devices": [
    {
      "id": "ABC123DEF456",
      "name": "iPhone 15",
      "model": "iPhone15,2",
      "osVersion": "iOS 18.1",
      "lastActivity": "2025-10-31T12:34:56Z",
      "trusted": true
    },
    ...
  ```

### Notes
