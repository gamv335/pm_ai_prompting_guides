# AI Prototyping Task Testing Prompt

Use this prompt after a task has been implemented.

The implementation plan should already contain the task’s acceptance criteria, review checkpoint, and testing checkpoint.

---

# Task Testing Prompt

Use the approved design document and implementation plan as the source of truth.

Provide testing instructions for the following task only:

Task ID or task name:
[Add task ID or task name]

Check the task against:

If you can run tests, run the relevant tests and report the results.

If you cannot run tests, provide clear manual testing instructions that I can follow.

After testing:

1. Summarise what was tested.
2. Report whether the task passed, partially passed, failed, or is blocked.
3. List any issues found.
4. Recommend fixes if needed.
5. Update the task status in the implementation plan:

   * ✅ Completed if it passed
   * 🟨 In Progress if it partially passed and needs fixes
   * ⛔ Blocked if it cannot be tested or completed
6. Add testing notes to the implementation plan.
7. Recommend the next task only if this one passed.

Stop after testing this task.

# Code Testing Prompt

Write test for the [file name, function, snippet, workflow] based on the requirements from Task ID [Number]. 

Run the tests and fix until all case pass.

# Bug Fix Testing Prompt

There's a bug: [Insert description]

Write a run failing tests that demonstrate the bug. 

Once the bug is fixes, write tests to ensure is fixed. 


