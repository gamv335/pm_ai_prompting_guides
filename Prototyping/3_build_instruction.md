# AI Prototyping Task Execution Prompt

Use this prompt after the design document and implementation plan have been approved.

The implementation plan should already contain enough detail for each task to be picked up immediately.

---

# Task Execution Prompt

Use the approved design document and implementation plan as the source of truth.

Implement the following task only:

Task ID or task name:
[Add task ID or task name]

Do not implement any other task.
Do not skip ahead.
Do not redesign the product.
Do not add unapproved features, dependencies, architecture, styling, data models, or integrations.

Before implementing, check the task’s dependencies, acceptance criteria, review checkpoint, and testing checkpoint in the implementation plan.

If the task is blocked, explain what is blocking it and stop.

After implementing:

1. Summarise what changed.
2. Explain how to test or review it.
3. Mark the task as completed in the implementation plan.
4. Add any implementation notes or follow-up tasks discovered.
5. Recommend the next task from the implementation plan, but do not start it.

Stop after this task.
