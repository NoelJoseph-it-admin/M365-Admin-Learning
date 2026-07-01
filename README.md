# M365-Admin-Learning
My hands-on Microsoft 365 Admin learning journey.
<h1 align="center">🖥️ Microsoft 365 Admin — Learning Journey</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Microsoft_365-Admin-blue?logo=microsoft&style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-In_Progress-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Sandbox-Developer_Tenant-green?style=for-the-badge" />
</p>

---

## 👤 About Me
- **Name:** Noel Roshen Joseph
- **Goal:** Learn Microsoft 365 Administration hands-on
- **Tenant:** admin194.onmicrosoft.com (Developer Sandbox)
- **Started:** June 2026

---

## 🗺️ Learning Roadmap

| # | Task | Category | Status |
|---|------|----------|--------|
| 1 | Employee Onboarding & Role Assignment | Users & Roles | ✅ Done |
| 2 | Distribution List & Shared Mailbox | Email & Groups | ✅ Done |
| 3 | Message Trace (Missing Email) | Exchange | ✅ Done |
| 4 | Recover Deleted User | Users | ✅ Done |
| 5 | Mail Forwarding | Exchange | ✅ Done |
| 6 | Reset MFA & Revoke Sessions | Entra ID | 🔄 In Progress |
| 7 | Restrict External Sharing (SharePoint) | SharePoint | ✅ Done |

---

## 📋 Task Details

### ✅ Task 1 — Employee Onboarding
**Admin Center:** Microsoft 365 Admin Center

**What I did:**
- Created user Jordan Taylor (`jtaylor@admin194.onmicrosoft.com`)
- Set Job Title: Helpdesk Specialist | Department: IT
- Assigned Microsoft 365 E5 Developer license
- Set temporary password with forced change on first login
- Assigned **Helpdesk Administrator** role

**What I learned:**
> Helpdesk Admin can reset passwords for regular users
> but cannot control the full tenant — principle of least privilege.

## 📸 Screenshots
### Task 1 — Creating Jordan Taylor
<img width="909" height="466" alt="add user" src="https://github.com/user-attachments/assets/59239db8-5276-436b-800e-51268865cd6d" />

---

### ✅ Task 2 — Email Groups & Shared Mailbox
**Admin Center:** Microsoft 365 Admin Center

| Feature | Distribution List | Shared Mailbox |
|---------|-------------------|----------------|
| Purpose | Broadcast to many | Team collaboration |
| Storage | No (uses member inboxes) | Yes (up to 50GB) |
| Reply As | Personal address | Shared address |
| Licensing | Free | Free |

**What I did:**
- Created Distribution List: `it-alerts@admin194.onmicrosoft.com`
  - Members: Admin + Jordan Taylor
- Created Shared Mailbox: `support@admin194.onmicrosoft.com`
  - Granted Jordan Taylor: Full Access + Send As

## 📸 Screenshots
### Task 2 — Email Groups & Shared Mailbox
<img width="917" height="469" alt="Dist List" src="https://github.com/user-attachments/assets/56dce29d-48f2-41c4-9bc9-3e0de7286170" />
<img width="916" height="467" alt="create mailbox" src="https://github.com/user-attachments/assets/06f448f4-a3fa-44d8-b05f-cfc08371bcbd" />


---

### ✅ Task 3 — Investigating Missing Email (Message Trace)
**Admin Center:** Exchange Admin Center

**Steps taken:**
1. Exchange Admin → Mail flow → Message trace
2. Set recipient: jtaylor@admin194.onmicrosoft.com
3. Date range: Last 2 days
4. Reviewed delivery status of messages

## 📸 Screenshots
### Task 3 — Investigating Missing Email (Message Trace)
<img width="910" height="470" alt="missing email trace" src="https://github.com/user-attachments/assets/05b9dcb4-0a27-4722-b9e6-643370376e28" />


---

### ✅ Task 4 — Recovering Deleted User
**Admin Center:** Microsoft 365 Admin Center

**Steps taken:**
1. Users → Deleted users
2. Located Jordan Taylor
3. Clicked Restore — account, mailbox and license restored

> 💡 Deleted users can be restored within 30 days
> before permanent deletion.

## 📸 Screenshots
### Task 4 — Recovering Deleted User
<img width="916" height="468" alt="user deletion" src="https://github.com/user-attachments/assets/67b74edd-ea62-438b-bc6f-4c297c6be7ca" />


---

### ✅ Task 5 — Mail Forwarding
**Admin Center:** Exchange Admin Center

**Steps taken:**
- Configured Jordan's mailbox to forward to `support@admin194.onmicrosoft.com`
- Enabled **"Keep a copy in Jordan's inbox"**

## 📸 Screenshots
### Task 5 — Mail Forwarding
<img width="915" height="467" alt="mail forwarding" src="https://github.com/user-attachments/assets/42246afc-3c85-4313-b981-2563383f7e3b" />

---

### 🔄 Task 6 — Reset MFA & Revoke Sessions
**Admin Center:** Microsoft Entra Admin Center

**Steps taken:**
- Enabled MFA for Jordan Taylor ✅
- Triggered "Require re-register MFA" 🔄 [In progress]
- Revoked all active sessions ✅

## 📸 Screenshots
### Task 6 — Reset MFA & Revoke Sessions
<img width="917" height="466" alt="session revoke" src="https://github.com/user-attachments/assets/18e2b52a-489e-4e98-aae7-ee3b9ba11f5b" />

---

### ✅ Task 7 — Restrict External Sharing (SharePoint)
**Admin Center:** SharePoint Admin Center

**Steps taken:**
- Located active site (Communication Site)
- Changed external sharing to: **Only people in your organization**

## 📸 Screenshots
### Task 7 — Restrict External Sharing
<img width="916" height="464" alt="external sharing" src="https://github.com/user-attachments/assets/a94f7f09-b58c-43f0-8bd9-02c9bbb26eb1" />

---

## 🧠 Key Concepts Learned

| Concept | Summary |
|---------|---------|
| Least Privilege | Give only the access needed, nothing more |
| Shared Mailbox | Free collaborative inbox, no licence needed |
| Distribution List | Email alias, no storage, broadcasts to members |
| MFA Reset | Done via Entra ID, not M365 Admin Center |
| Message Trace | Exchange tool to track email delivery status |
| Soft Delete | Deleted users recoverable within 30 days |

---

## 🛠️ Admin Centers Used

| Admin Center | URL |
|---|---|
| Microsoft 365 | admin.microsoft.com |
| Exchange | admin.exchange.microsoft.com |
| Entra ID | entra.microsoft.com |
| SharePoint | admin.microsoft.com/sharepoint |

---

<p align="center">
  <i>Built with 💙 while learning Microsoft 365 Administration</i>
</p>
