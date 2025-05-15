
# 🌱 TreeTracker + Hyperledger Fabric Integration - Jira Agile User Stories

This archive contains the **complete Jira Agile user stories**, broken down into **Scrum-ready tasks**, for integrating the TreeTracker App with Hyperledger Fabric (HLF).

---

## ✅ Jira Agile User Stories

### 🧩 Epic: Tree Verification & Blockchain Integration

**Epic Description:**
Enable secure, decentralized tracking of tree planting data using Hyperledger Fabric for transparency, fraud prevention, and token-based incentives.

---

### 🟦 Story 1: Set Up Hyperledger Fabric Network
**As a** blockchain engineer,  
**I want to** deploy a Hyperledger Fabric network  
**So that** we can securely track tree planting records.

**Acceptance Criteria:**
- Fabric network includes orderers and peers
- Certificate Authorities (CAs) are operational
- Channels are configured

**Sub-tasks:**
- Install prerequisites (Docker, Go, Node.js)
- Set up Fabric network (orderer + peer services)
- Package and install smart contracts
- Approve and commit chaincode to the network

📅 Sprint: 1 | 📌 Priority: Highest | 👤 Assignee: DevOps & Blockchain Engineer | 📊 Story Points: 8

---

### 🟦 Story 2: Offline Tree Data Capture
**As a** smallholder farmer,  
**I want to** capture tree planting data offline (photo, GPS, metadata)  
**So that** I can record tree planting efforts without needing internet.

**Acceptance Criteria:**
- UI for photo + metadata input
- Data stored locally offline
- Auto-sync when online

**Sub-tasks:**
- Design UI for capturing tree photo
- Add metadata fields (species, notes, GPS)
- Implement local storage (SQLite or IndexedDB)
- Build sync queue for offline data

📅 Sprint: 1 | 📌 Priority: High | 👤 Assignee: Mobile App Developer | 📊 Story Points: 5

---

### 🟦 Story 3: Automatic Data Sync
**As a** farmer,  
**I want to** auto-upload offline data when I regain connectivity  
**So that** I don’t have to manually manage it.

**Acceptance Criteria:**
- App detects internet connection
- Pending offline data is synced
- UI confirms upload

**Sub-tasks:**
- Develop network detection logic
- Create sync service (background process)
- Add upload status indicators to UI
- Notify users on sync success/failure

📅 Sprint: 2 | 📌 Priority: Medium | 👤 Assignee: Backend Engineer | 📊 Story Points: 5

---

### 🟦 Story 4: Tree Submission Blockchain Record
**As a** verifier,  
**I want to** immutably store submissions on Hyperledger Fabric  
**So that** data is secure and tamper-proof.

**Acceptance Criteria:**
- Verified data added to blockchain
- Record includes ID, GPS, timestamp
- Retrievable via API

**Sub-tasks:**
- Define on-chain data schema (tree ID, planter ID, etc.)
- Implement smart contract for submission recording
- Create API to query blockchain records

📅 Sprint: 2 | 📌 Priority: High | 👤 Assignee: Blockchain Developer | 📊 Story Points: 8

---

### 🟦 Story 5: Tree Submission Validation
**As a** validator,  
**I want to** validate submissions using smart contracts  
**So that** invalid or duplicate data is rejected.

**Acceptance Criteria:**
- GPS must be within allowed zones
- Duplicates are flagged
- Image quality is checked

**Sub-tasks:**
- Add GPS validation logic in smart contract
- Check for duplicate tree submissions
- Integrate AI to assess photo clarity
- Flag poor-quality images

📅 Sprint: 3 | 📌 Priority: Critical | 👤 Assignee: Blockchain & AI Engineers | 📊 Story Points: 8

---

### 🟦 Story 6: Token Minting for Verified Trees
**As a** farmer,  
**I want to** earn Impact Tokens for verified trees  
**So that** I’m rewarded for reforestation.

**Acceptance Criteria:**
- Verified trees trigger token minting
- Tokens visible in user wallet
- Token value rules enforced

**Sub-tasks:**
- Smart contract logic for minting tokens
- Define token structure (ID, owner, value)
- UI to show balance and token history

📅 Sprint: 3 | 📌 Priority: High | 👤 Assignee: Blockchain Smart Contract Developer | 📊 Story Points: 5

---

### 🟦 Story 7: Tree Growth Verification
**As a** farmer,  
**I want to** get alerts for tree survival checks  
**So that** I can update the system and earn continued rewards.

**Acceptance Criteria:**
- Notifications for follow-up checks
- Photo uploads linked to existing trees
- Blockchain updated after verification

**Sub-tasks:**
- Enable push/email alerts for check-ins
- Build UI for submitting follow-up photos
- Update smart contract logic with survival status
- Adjust token balance based on tree survival

📅 Sprint: 4 | 📌 Priority: Medium | 👤 Assignee: Mobile App & Blockchain Developers | 📊 Story Points: 5

---

## ✅ Summary Table

| Story Name                       | Points | Sprint | Priority | Component     |
|----------------------------------|--------|--------|----------|---------------|
| HLF Network Setup                | 8      | 1      | Highest  | Blockchain    |
| Offline Tree Data Capture        | 5      | 1      | High     | Mobile App    |
| Automatic Data Sync              | 5      | 2      | Medium   | Backend       |
| Blockchain Record Creation       | 8      | 2      | High     | Blockchain    |
| Smart Contract-Based Validation  | 8      | 3      | Critical | Blockchain/AI |
| Token Minting for Verified Trees | 5      | 3      | High     | Blockchain    |
| Tree Growth Verification         | 5      | 4      | Medium   | Mobile + BC   |
