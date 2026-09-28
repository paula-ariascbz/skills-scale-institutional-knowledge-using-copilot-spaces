# Custom Chat Modes Guide

This repository includes specialized chat modes for GitHub Copilot that provide contextual guidance on OctoAcme processes. These modes shape how Copilot analyzes and responds to questions about our project management framework.

## 🎯 Available Chat Modes

Each mode is located in `.github/chatmodes/` and is automatically available in Copilot when working with this repository.

### 1. **Process Analyzer** 
**File:** `.github/chatmodes/process-analyzer.md`

**When to use:**
- Deep-dive reviews of process effectiveness
- Identifying gaps or inconsistencies in workflows
- Planning process improvements or re-tooling
- Onboarding senior team members or leads
- Pre-mortem analysis before large initiatives

**Example questions:**
- "What are the failure modes in our current process?"
- "Where do decision-making accountability gaps exist?"
- "How would a new team member misunderstand our project execution?"
- "What's missing from our escalation framework?"
- "Which personas are overloaded or underutilized?"

---

### 2. **Decision Framework**
**File:** `.github/chatmodes/decision-framework.md`

**When to use:**
- Making critical project or process decisions
- Evaluating trade-offs and options
- Aligning stakeholders on major choices
- Documenting decision rationale for future learning
- Assessing reversibility ("one-way door" vs. "two-way door")

**Example questions:**
- "Should we extend the timeline?"
- "Do we need to add resources or reduce scope?"
- "How do we decide if we're done with a feature?"
- "Is this a project we should take on?"
- "Which option best fits our principles?"

---

### 3. **Risk Auditor**
**File:** `.github/chatmodes/risk-auditor.md`

**When to use:**
- Risk identification and planning for new projects
- Weekly/bi-weekly risk register reviews
- Post-incident root-cause analysis
- Dependency audits before cross-team coordination
- Pre-mortem or failure-mode analysis
- Contingency planning for high-stakes initiatives

**Example questions:**
- "What could go wrong with this project?"
- "Build a risk register for [project type]"
- "How resilient is our rollback process?"
- "Where is single-person dependency highest?"
- "What assumptions are we making that could break?"

---

### 4. **Team Onboarding**
**File:** `.github/chatmodes/team-onboarding.md`

**When to use:**
- Onboarding new team members or leaders
- Explaining process rationale to new roles
- Tailoring guidance based on role and experience
- Helping teams adapt OctoAcme practices to their context
- Mentoring junior PMs or product folks
- Facilitating process adaptation discussions

**Example questions:**
- "What's expected of me during planning?"
- "How detailed should my PR descriptions be?"
- "What does 'Definition of Done' mean?"
- "How do I write a good One-pager?"
- "When is scope change approval needed?"

---

## 🚀 How to Use Chat Modes

### In VS Code (with Copilot Chat enabled)

1. Open a conversation in GitHub Copilot Chat
2. Look for the mode selector (appears as a dropdown or button)
3. Select the mode that matches your task:
   - **Process Analyzer** — for process improvement analysis
   - **Decision Framework** — for decision-making guidance
   - **Risk Auditor** — for risk identification and management
   - **Team Onboarding** — for learning and mentoring

4. Ask your question — Copilot will use the mode's context to shape its response

### Example Workflow

**Scenario:** You're planning a data migration project and want to identify risks.

1. Open Copilot Chat
2. Select **Risk Auditor** mode
3. Ask: "Build a risk register for a data migration. We have 1 DBA, production is 10TB, and we need to roll back if something fails."
4. Copilot will provide:
   - Specific risk categories (technical, organizational, schedule)
   - Impact/likelihood assessment
   - Mitigation strategies
   - Contingency planning

---

## 📋 Mode Features

Each mode includes:

- **System Context** — Expertise and perspective the mode embodies
- **Key Documents** — Which OctoAcme docs the mode references
- **Analysis Categories** — Frameworks for thinking about the topic
- **Example Prompts** — Questions you're likely to ask
- **Output Guidelines** — How responses should be structured
- **When to Use** — Situations where this mode is most helpful

---

## 🔧 Customizing or Creating New Modes

Modes are Markdown files in `.github/chatmodes/`. Each file contains:

1. **Purpose** — What the mode helps with
2. **System Context** — Expert persona and expertise areas
3. **Your Role** — What the mode does when activated
4. **Key Frameworks/Documents** — Resources and reference materials
5. **Analysis Approach** — Step-by-step thinking
6. **Prompts You Might Receive** — Common use cases
7. **Output Guidelines** — Quality and format expectations
8. **When to Use** — Situations calling for this mode

### To Create a New Mode

1. Create a new `.md` file in `.github/chatmodes/`
2. Follow the template structure above
3. Tie it to OctoAcme processes in `docs/`
4. Commit and it will automatically be available in Copilot Chat

---

## 💡 Tips for Best Results

### Ask Specific Questions
❌ "Tell me about our processes"  
✅ "Where might single-person dependencies create risk?"

### Provide Context
❌ "How do we make decisions?"  
✅ "We're deciding whether to delay release by 1 week for testing. How should we evaluate this?"

### Reference Artifacts
❌ "What's in a good risk register?"  
✅ "Review our risk register from the last project and suggest improvements"

### Combine Modes
Use multiple modes for complex topics:
- Start with **Team Onboarding** to understand a process
- Use **Decision Framework** to evaluate options
- Apply **Risk Auditor** to stress-test the decision

---

## 🎓 Learning Paths by Role

### For Developers
1. **Team Onboarding** — "What's expected of me in planning?"
2. **Process Analyzer** — "How do we handle escalations?"
3. **Risk Auditor** — "What test coverage is needed?"

### For Project/Product Managers
1. **Team Onboarding** — "How do I write a One-pager?"
2. **Decision Framework** — "Should we extend timeline?"
3. **Risk Auditor** — "Build a risk register for this project"
4. **Process Analyzer** — "Where are our process gaps?"

### For Leads/Stakeholders
1. **Team Onboarding** — "What information do I need for approval?"
2. **Decision Framework** — "How are escalations made?"
3. **Risk Auditor** — "What should I look for in project health?"

### For New Team Members
1. **Team Onboarding** — "How is work prioritized?"
2. **Team Onboarding** — "What does success look like?"
3. Any mode — Ask role-specific questions as they arise

---

## 🔗 Resources

- **OctoAcme Process Docs** — See `docs/README.md`
- **Copilot Chat Documentation** — [GitHub Copilot Docs](https://docs.github.com/en/copilot)
- **Copilot Spaces** — [Using Copilot Spaces](https://docs.github.com/en/copilot/how-tos/provide-context/use-copilot-spaces/)

---

**Last Updated:** 2026-09-28  
**Questions?** Open an issue in this repository with feedback or suggestions for new modes.
