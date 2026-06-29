# AI Prototyping Implementation Plan Prompt

Use this prompt after the design document has been reviewed and approved.

The purpose of this stage is to turn the approved design document into a practical build plan. The AI should not redesign the product, duplicate the design document, invent new features, or start coding.

The approved design document is the source of truth. The implementation plan should explain how to build it in a logical, testable sequence.

---

# Implementation Plan Prompt

I have approved the design document attached.

Now create a practical implementation plan for building it.

Do not start building yet.
Do not write code yet.
Do not generate final screens yet.
Do not redesign the product.
Do not duplicate or rewrite the design document.

Use the approved design document as the source of truth. Reference it where needed, but do not restate it in full.

If anything in the design document is unclear or blocks implementation planning, ask focused questions before creating the plan. If a reasonable assumption is needed, label it clearly as an assumption and explain why it is needed.

Do not add new features, user roles, flows, integrations, data models, visual styles, architecture, dependencies, or technical complexity unless they are necessary to implement the approved design. If you recommend anything new, clearly mark it as a recommendation and explain why it is needed.

The styling notes, visual direction, component guidance, accessibility requirements, and design-system requirements in the approved design document are part of the build scope. They must be carried into the implementation plan and reflected in the build tasks.

---

## Your task

Create an implementation plan that breaks the approved design into a logical sequence of bite-sized tasks or milestones.

Do not summarise the full design document. Instead, use short references such as:

* “Based on the approved main user journey…”
* “From the approved styling requirements…”
* “From the approved data requirements…”
* “From the approved edge cases…”

The plan should be detailed enough that a developer, designer, or AI coding/prototyping tool can work through it step by step.

The plan should avoid vague tasks such as “build the app” or “create the UI”. Each task should produce something specific that can be reviewed, tested, or approved.

---

## The implementation plan should include

### 1. Implementation overview

Briefly explain:

* The build approach
* The recommended order of work
* What will be mocked, simplified, or deferred
* Any implementation blockers or questions

Keep this concise. Do not repeat the design document.

### 2. Planning assumptions and blockers

List only the assumptions or blockers that affect the implementation plan.

Separate:

* Confirmed source-of-truth items from the design document that affect sequencing
* Assumptions needed to create the plan
* Open questions that may block implementation

Do not restate all product requirements.

### 3. Build scope

Define the build scope using the approved design document as the reference.

Separate:

* Build now
* Build later
* Do not build

Keep each item short and implementation-focused.

### 4. Plan

Break the work into milestones.

For each milestone, include:

* Milestone name
* Purpose
* What will be created
* Dependency
* Expected output
* Review checkpoint
* Testing checkpoint

Each milestone should be small enough to review meaningfully.

For each milestone, break the work into small, specific tasks.

For each task, include:

* Task ID
* Task name
* What will be created or changed
* Why it is needed
* Source reference from the design document
* Expected output
* Acceptance criteria
* Review checkpoint
* Testing checkpoint

Use concise references to the design document rather than copying sections from it.

Explain the logical order of work.

The sequence should usually move from foundation to user-facing experience:

1. Project setup or file structure
2. Design tokens, styling foundations, or theme setup
3. Mock data or data structures
4. Core layout and navigation
5. Main screens or user flows
6. Key components
7. States and edge cases
8. Accessibility and responsive behaviour
9. Testing and review
10. Final refinement


### 5. Testing checkpoints

Turn the approved testing strategy into practical checkpoints throughout the build.

Include only relevant checks, such as:

Testing should appear throughout the implementation plan, not only at the end.

### 6. Definition of done

Define what must be true before the implementation is considered complete.

Include only criteria tied to the approved design document and this implementation plan.


### 7. Risks and watchouts

Identify where the build could drift from the approved design document.

Include risks such as:

* Adding unapproved features
* Duplicating or rewriting the design instead of implementing it
* Ignoring styling requirements
* Over-engineering the stack
* Creating unnecessary backend complexity
* Losing accessibility requirements
* Missing edge cases
* Treating mock data as real architecture
* Building screens before foundations are clear
* Skipping review checkpoints

### 8. Final approval checkpoint

End by asking me to review, adjust, or approve the implementation plan.

Important: stop after producing the implementation plan. Do not start coding, generating final screens, or building the prototype until I approve the plan.

---

# Recommended Step 2 Workflow

```text
Approved design document
→ AI checks for unclear or blocking implementation details
→ AI creates implementation plan using the design document as reference
→ Human reviews and edits
→ Implementation plan is approved
→ Build starts one task at a time
```

---

# Key Principle

The design document decides what should exist.

The implementation plan decides how to build it.

Do not duplicate the design document inside the implementation plan. Reference it, sequence it, and turn it into buildable tasks.
