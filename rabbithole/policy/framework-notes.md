---
description: >-
  Personal design notes for building a simple, extensible framework for
  developing metagovernace working groups
---

# Metagov Documentation Framework Notes

🔎[️ v0 Reference Implementation](https://v0.rabbithole.rathermercurial.xyz)\
[✒️ v0 Document Archive (WIP)](https://sandbox.rabbithole.rathermercurial.xyz)

Designed by [rathermercurial.eth](https://rathermercurial.eth.xyz)

In documenting RabbitHole Metagovernance Pod v0, it was necessary to build a basic documentation framework to organize metagov information in a comprehensible manner. These are notes related to its design.

### 💭 Project Summary

The Metagovernance Documentation Framework is a simple file structure and ruleset for storing metagovernance pod information. All policies, processes and activity are recorded as markdown files in an open-source git repository, and displayed in an attractive, human-readable format on GitBook.

Voting workstream activities are separated logically by concern and organized hierarchically to create a modular, extensible framework for organizing information related to metagov working groups.

Git-based source control allows for regular, trouble-free updates to the entire metagovernance process with no transition periods, downtime, or breaking changes to the UX.

#### 🏃 Based on existing agile governance development principles

* Predictable Release (Upgrade) Cycle with Test & Dev Branches.
* Combines regular stable release schedule with CI/CD "Move Fast and Fix Things" development backend.
* Built around best practices so as to be Peer-Reviewable and Formally Verifiable.
* Workflow-Agnostic for use across verticals, platforms and paradigms.

#### 🧱 Modular and extensible design

* Each pod owns its policies and best practices. Pods are plug-and-play, composable and seamlessly divorceable.
* Can be vertically scaled using pages and folders (aligned with pods, inspired by Orca).
* Can be horizontally scaled using subfolders (aligned with domain / roles).

#### 🤝 Alignment with RabbitHole's business model and values

* Clearly described policies and practices help inform and align parallel workstreams.
* Speeds time to market by reducing primitives needed to deploy liquid human capital.
* Dedicated development pipeline abstracts complex, time-consuming tasks away from other workstreams.

### 📅 Timeline

Since this framework is relatively conventional, a timeline for bootstrapping it into production can be reasonably estimated:

#### Season 0

* Develop Metagov Framework v0

#### Season 1

* Begin Metagov Pod v1 +
* Bootstrap Metagov Framework v0
* Buidl Metagov Framework v1 (alpha)

... and so on.

### 📝 Other Notes

* The "activity" folder is a temporary solution for the publication of voting workstream activity. Future iterations should leverage IPFS, Ceramic streams or another contemporary storage solution.
