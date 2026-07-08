# Inbound Software - New Test Tool Request Workflow

---

## Slide 1: Workflow Overview

### Inbound Software - New Test Tool Request Workflow

**Purpose:** Manage and streamline requests for new test tools from DSV test manager through approval and registration

**Key Stakeholders:**
- DSV Test Manager (Initiator)
- QA Core (Assessor & Researcher)
- QA Chapter (Approver)
- EA Team (Registrar)

---

## Slide 2: Process Flow Diagram

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                                                                               │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │  DSV Test Manager                                                    │   │
│  │  Raises Request for New Test Tool                                    │   │
│  └────────────────────┬─────────────────────────────────────────────────┘   │
│                       │                                                      │
│                       ▼                                                      │
│  ┌──────────────────────────────────────────────────────────────────────┐   │
│  │  QA Core Reviews Request                                             │   │
│  └────────────────────┬─────────────────────────────────────────────────┘   │
│                       │                                                      │
│                       ▼                                                      │
│        ┌──────────────────────────────────┐                                 │
│        │  Tool Exists in DSV Test         │                                 │
│        │  Tool Pool?                      │                                 │
│        └──────────┬──────────────┬────────┘                                 │
│                   │              │                                          │
│            YES ◄──┘              └──► NO                                    │
│                   │                     │                                   │
│                   ▼                     ▼                                   │
│  ┌─────────────────────────┐  ┌──────────────────────────────────────┐     │
│  │ QA Core Provides        │  │ QA Core Conducts Tool Research       │     │
│  │ Recommendation          │  │ - Evaluate capabilities              │     │
│  │ Close Request           │  │ - Check compatibility                │     │
│  └─────────────────────────┘  │ - Assess cost & licensing            │     │
│                                │ Prepare Recommendation Document      │     │
│                                └────────────┬─────────────────────────┘     │
│                                             │                               │
│                                             ▼                               │
│                        ┌────────────────────────────────────────┐            │
│                        │  QA Chapter Reviews Recommendation      │            │
│                        │  Evaluates against organizational       │            │
│                        │  standards and best practices           │            │
│                        └────────────┬──────────────┬─────────────┘            │
│                                     │              │                         │
│                              REJECTED             APPROVED                   │
│                                     │              │                         │
│                                     ▼              ▼                         │
│                        ┌────────────────────┐  ┌──────────────────────────┐ │
│                        │ Close Request      │  │ QA Core Contacts EA Team │ │
│                        │ with Feedback      │  └────────────┬─────────────┘ │
│                        └────────────────────┘               │                │
│                                                             ▼                │
│                                        ┌────────────────────────────────┐   │
│                                        │ EA Team Registers Tool         │   │
│                                        │ in System                      │   │
│                                        └────────────┬───────────────────┘   │
│                                                     │                       │
│                                                     ▼                       │
│                                        ┌────────────────────────────────┐   │
│                                        │ Tool Added to DSV Test         │   │
│                                        │ Tool Pool                      │   │
│                                        └────────────┬───────────────────┘   │
│                                                     │                       │
│                                                     ▼                       │
│                                        ┌────────────────────────────────┐   │
│                                        │ Request Closed Successfully    │   │
│                                        │ Stakeholders Notified          │   │
│                                        └────────────────────────────────┘   │
│                                                                              │
└──────────────────────────────────────────────────────────────────────────────┘
```

---

## Slide 3: Workflow Stages - Detailed Breakdown

### **Stage 1: Request Initiation**
- **Actor:** DSV Test Manager
- **Action:** Identify need for new test tool and raise formal request
- **Output:** Formal request with tool requirements and use case

### **Stage 2: Initial Assessment**
- **Actor:** QA Core
- **Action:** Review request and check if tool exists in DSV test tool pool
- **Decision:** Tool exists or not?

### **Stage 3: Tool Research & Recommendation**
- **Actor:** QA Core
- **Activities:**
  - Conduct comprehensive tool research
  - Evaluate capabilities and compatibility
  - Assess cost, licensing, and maintenance
  - Prepare recommendation document
- **Output:** Detailed recommendation ready for approval

### **Stage 4: Review & Approval**
- **Actor:** QA Chapter
- **Action:** Review tool against organizational standards
- **Decision:** Approve or reject recommendation

### **Stage 5: Tool Registration**
- **Actor:** QA Core + EA Team
- **Activities:**
  - QA Core contacts EA team with approval
  - EA team registers tool in system
  - Tool added to DSV test tool pool
  - Notify all stakeholders
- **Output:** Tool live in DSV test tool pool

---

## Slide 4: Key Decision Points & Outcomes

### **Decision Point 1: Tool Pool Check**
```
Question: Tool Exists in DSV Test Tool Pool?
├─ YES  → Provide recommendation & Close (Fast Track)
└─ NO   → Proceed to Research Phase
```

### **Decision Point 2: QA Chapter Approval**
```
Question: Tool Approved by QA Chapter?
├─ YES  → Proceed to EA Registration
└─ NO   → Close with Feedback to Requester
```

---

## Slide 5: Success Criteria & Outcomes

### ✓ Success Criteria

- ✓ Tool research is thorough and documented
- ✓ QA Chapter approval obtained before EA registration
- ✓ Tool successfully registered in system
- ✓ All stakeholders notified of completion
- ✓ Tool available in DSV test tool pool

### Timeline Expectations

| Stage | Typical Duration |
|-------|------------------|
| Request Review | 2-3 business days |
| Tool Research | 5-10 business days |
| QA Chapter Review | 3-5 business days |
| EA Registration | 2-3 business days |
| **Total** | **12-21 business days** |

---

## Slide 6: Responsible Parties & Handoffs

| Stage | Responsible Party | Hands Off To |
|-------|------------------|--------------|
| Initiation | DSV Test Manager | QA Core |
| Assessment | QA Core | QA Core (if research needed) |
| Research | QA Core | QA Chapter |
| Approval | QA Chapter | QA Core |
| Registration | QA Core + EA Team | Complete |

---

## Slide 7: Contact & Support

**Questions or Issues?**

- **For Request Status:** Contact QA Core
- **For Tool Integration:** Contact EA Team
- **For Workflow Questions:** Contact QA Chapter Lead

**Key Contacts:**
- QA Core Lead: [TBD]
- QA Chapter Lead: [TBD]
- EA Team: [TBD]
