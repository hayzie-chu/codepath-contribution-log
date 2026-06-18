# Contribution 2: Update Agent Counter 

**Contribution Number:** 2
**Student:** Nhi Chu (Hayzie)
**Issue:** [https://github.com/Portabase/portabase/issues/271]
**Status:** [Phase II] [In progress]

---

## Why I Chose This Issue

I chose this issue because it's on the same repo that I have been contributing to, so I am familiar with the codebase and the tech stack used. 
This would also be a good practice on Javascript and full-stack development, especially on real-world debugging problems.
The issue is also clearly described and seems to be related to the files I have worked with in my previous contribution. 
It also has a clear way to double check whether my contribution fixes the problem visually, by replicating the problem.

---

## Understanding the Issue

### Problem Description

The Agent count display is not updated correctly in the case where an user deletes an existing agent. 

### Expected Behavior

The Agent counter should decrement whenever the user deletes an agent on the UI and display the updated count.

### Current Behavior

The counter stays the same, and still counts the deleted agent. But adding a new agent still updates it correctly.

### Affected Components

app/(customer)/dashboard/home/page.tsx
app/(customer)/dashboard/(admin)/agents

---

## Reproduction Process

### Environment Setup

The same process as [https://github.com/hayzie-chu/opensource-contribution-log/blob/main/Portabase-Google-Cloud.md]

### Steps to Reproduce

1. Clone and cd into the repo
2. Start up Docker
3. Install dependencies: pnpm install
4. Environment configuration: cp .env.example .env
5. Start postgres: docker compose up -d
6. Start in development mode: make up
7. Go to http://localhost:8887
8. Log in using the provided example default account
9. Navigate to Administration/Agents on the left panel
10. Add agent(s)
11. Navigate back to Home Dashboard to check the number of Agents (should be correct)
12. Navigate back to Agents page and delete the client
13. Navigate back to Home Dashboard to check the number of Agents (should be incorrect and has not changed)

### Reproduction Evidence

- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach

### Analysis

[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution

[High-level description of your fix approach]

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]
1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
