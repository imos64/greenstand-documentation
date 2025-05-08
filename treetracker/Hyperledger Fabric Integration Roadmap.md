
# 🌿 Treetracker + Hyperledger Fabric Integration Roadmap

This document outlines the Jira-standard roadmap for integrating the Treetracker Android app with a Hyperledger Fabric blockchain network.

---

## 🧱 EPIC 1: Blockchain Network Setup

| Story | Description | Est. Sprint |
|-------|-------------|-------------|
| FAB-1 | Set up development Fabric network with 2 orgs (Growers, Verifiers) | Sprint 1 |
| FAB-2 | Write chaincode: `SubmitTreeCapture`, `VerifyCapture`, `IssueToken` | Sprint 1–2 |
| FAB-3 | Create Fabric CA and enroll users | Sprint 2 |
| FAB-4 | Unit test all chaincode functions | Sprint 2 |

---

## 🧱 EPIC 2: Middleware API Development

| Story | Description | Est. Sprint |
|-------|-------------|-------------|
| MID-1 | Create API endpoints: `submitTree`, `getTreeStatus`, `getTokens` | Sprint 2 |
| MID-2 | Integrate HLF SDK to interact with blockchain | Sprint 2 |
| MID-3 | Add IPFS upload support for image files | Sprint 3 |
| MID-4 | Add JWT-based authentication for API | Sprint 3 |
| MID-5 | Write API unit and integration tests | Sprint 3 |

---

## 🧱 EPIC 3: Android App Refactor

| Story | Description | Est. Sprint |
|-------|-------------|-------------|
| APP-1 | Remove RetrofitAPI, Firebase, and AWS | Sprint 2 |
| APP-2 | Create `HLFAPI.kt` to call middleware | Sprint 3 |
| APP-3 | Create `IPFSService.kt` to upload image and get hash | Sprint 3 |
| APP-4 | Implement `CaptureHasher.kt` for SHA-256 image hashing | Sprint 3 |
| APP-5 | Modify `DataSync.kt` to use blockchain flow | Sprint 4 |
| APP-6 | Add UI for verification status & token balance | Sprint 4 |

---

## 🧱 EPIC 4: Testing & Deployment

| Story | Description | Est. Sprint |
|-------|-------------|-------------|
| TST-1 | End-to-end test: capture → verify → token | Sprint 4 |
| TST-2 | Load test chaincode and middleware API | Sprint 4 |
| TST-3 | Deploy Fabric to staging / production | Sprint 5 |
| TST-4 | Release updated app to testers | Sprint 5 |

---

## 🗓️ Sprint Summary

| Sprint | Focus |
|--------|-------|
| Sprint 1 | Fabric setup, chaincode dev |
| Sprint 2 | CA & API scaffolding, Android cleanup |
| Sprint 3 | Middleware & Android blockchain integration |
| Sprint 4 | Full integration & UI updates |
| Sprint 5 | Deployment & release |
| Sprint 6 | Bug fixes & feedback loop |

---
