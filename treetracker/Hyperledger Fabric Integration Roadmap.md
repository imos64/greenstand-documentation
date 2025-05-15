# TreeTracker App + Hyperledger Fabric Integration Roadmap

## 🚀 Jira Agile Roadmap Overview

This roadmap breaks down the integration of the TreeTracker App with Hyperledger Fabric blockchain into Epics, Milestones, and Sprints using Scrum methodology.

---

### 🧩 EPIC 1: Blockchain Infrastructure Setup

**Goal:** Deploy a scalable, secure HLF network to support blockchain-based tree verification.

| Sprint | Milestone                 | User Stories                                      | Roles                       | Status |
| ------ | ------------------------- | ------------------------------------------------- | --------------------------- | ------ |
| 1      | Deploy Hyperledger Fabric | ✅ Set up HLF network with CA, Orderers, and Peers | DevOps, Blockchain Engineer | To Do  |
| 1      | Chaincode framework ready | ✅ Install base chaincode templates                | Blockchain Engineer         | To Do  |

---

### 🧩 EPIC 2: Tree Data Capture & Offline Sync

**Goal:** Enable farmers to submit geo-tagged tree data even without internet access.

| Sprint | Milestone                         | User Stories                                 | Roles               | Status      |
| ------ | --------------------------------- | -------------------------------------------- | ------------------- | ----------- |
| 1      | Local Data Capture (Offline Mode) | ✅ Capture photo, GPS, metadata offline       | Mobile Dev          | In Progress |
| 2      | Sync Mechanism                    | ✅ Auto-upload tree data when online          | Mobile, Backend Dev | To Do       |
| 2      | User Feedback                     | ✅ Upload status and success/failure messages | Frontend Dev        | To Do       |

---

### 🧩 EPIC 3: Blockchain Integration for Verified Trees

**Goal:** Record valid tree data on-chain for immutability and transparency.

| Sprint | Milestone                          | User Stories                                    | Roles              | Status |
| ------ | ---------------------------------- | ----------------------------------------------- | ------------------ | ------ |
| 2      | On-Chain Record Storage            | ✅ Record verified trees on blockchain           | Blockchain Dev     | To Do  |
| 3      | Data Validation via Smart Contract | ✅ Validate GPS, metadata, and detect duplicates | Blockchain, AI Eng | To Do  |
| 3      | Image Quality Verification         | ✅ AI-powered photo clarity check                | AI Engineer        | To Do  |

---

### 🧩 EPIC 4: Token Incentive System

**Goal:** Issue tokens to planters based on verified tree submissions.

| Sprint | Milestone                        | User Stories                            | Roles                         | Status |
| ------ | -------------------------------- | --------------------------------------- | ----------------------------- | ------ |
| 3      | Smart Contract for Token Minting | ✅ Token generation on tree verification | Blockchain Smart Contract Dev | To Do  |
| 3      | Wallet Integration               | ✅ Display user tokens and history       | Frontend Dev, Blockchain Dev  | To Do  |

---

### 🧩 EPIC 5: Post-Planting Monitoring

**Goal:** Verify tree survival over time and adjust rewards accordingly.

| Sprint | Milestone               | User Stories                                   | Roles          | Status |
| ------ | ----------------------- | ---------------------------------------------- | -------------- | ------ |
| 4      | Notification System     | ✅ Alert users for survival check submissions   | Mobile Dev     | To Do  |
| 4      | Follow-up Image Capture | ✅ Allow submission of new tree photos          | Mobile Dev     | To Do  |
| 4      | Blockchain Update       | ✅ Update smart contract and adjust token value | Blockchain Dev | To Do  |

---

## 📅 Sprint Timeline (4-Week Cycles)

| Sprint   | Dates (Suggested) | Focus Area                                  |
| -------- | ----------------- | ------------------------------------------- |
| Sprint 1 | Week 1–2          | Blockchain infrastructure + Offline Capture |
| Sprint 2 | Week 3–4          | Sync + Blockchain Record Creation           |
| Sprint 3 | Week 5–6          | Smart Contract Validation + Token Minting   |
| Sprint 4 | Week 7–8          | Survival Checks + Monitoring Logic          |

---

## 🧩 Jira Components Mapping

| Component       | Description                                         |
| --------------- | --------------------------------------------------- |
| `Blockchain`    | All smart contracts, HLF deployment, on-chain logic |
| `Mobile App`    | Data capture, UI for users, offline handling        |
| `Backend`       | APIs, sync services, network status detection       |
| `AI/Validation` | Image validation, duplicate detection               |
| `Wallet`        | Token balance display, transaction log              |

---

**Prepared for Agile Scrum implementation of TreeTracker + Hyperledger Fabric integration.**

---

