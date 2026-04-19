# Advanced Tricks & Edge Cases (Level 27–34)

This section focuses on less predictable challenges that require careful reading and attention to detail.  
It introduces version control (Git) and reinforces the idea that simple clues are often hidden in plain sight.

---

## Level 27

**Goal:**  
Retrieve data from a Git repository.

**Concept:**  
Basic Git usage.

**Approach:**  
Cloned the repository using `git clone`, then explored its contents to find useful information.

**Why it works:**  
Git repositories store files and history locally once cloned, allowing full inspection.

**Key Takeaway:**  
Sometimes the data isn’t hidden—it’s just in a different system (like version control).

---

## Level 28

**Goal:**  
Find sensitive data in repository history.

**Concept:**  
Git commit history.

**Approach:**  
Used `git log` and inspected previous commits to locate information that was removed in later versions.

**Why it works:**  
Git keeps a full history of changes, even if data is deleted later.

**Key Takeaway:**  
Deleting something doesn’t mean it’s gone—history matters.

---

## Level 29

**Goal:**  
Explore different branches for hidden data.

**Concept:**  
Git branches.

**Approach:**  
Listed branches using `git branch -a` and switched between them to check for hidden information.

**Why it works:**  
Different branches can contain different versions of files.

**Key Takeaway:**  
Always check all available paths—not just the default one.

---

## Level 30

**Goal:**  
Retrieve data from tags.

**Concept:**  
Git tags.

**Approach:**  
Used `git tag` to list tags and inspected them to find stored information.

**Why it works:**  
Tags can reference specific commits and may contain useful data.

**Key Takeaway:**  
Metadata (like tags) can hold important clues.

---

## Level 31

**Goal:**  
Push changes to a repository under specific conditions.

**Concept:**  
Git interaction and restrictions.

**Approach:**  
Followed instructions in the repository, made required changes, and pushed them to trigger the next step.

**Why it works:**  
Some systems validate actions based on repository changes.

**Key Takeaway:**  
Understanding instructions carefully is sometimes all that’s needed.

---

## Level 32

**Goal:**  
Escape a restricted shell using available commands.

**Concept:**  
Command restrictions and bypassing them.

**Approach:**  
Identified allowed commands and used them creatively to spawn a usable shell.

**Why it works:**  
Even restricted environments often leave indirect ways to execute commands.

**Key Takeaway:**  
Restrictions are rarely perfect—look for indirect execution paths.

---

## Level 33

**Goal:**  
Retrieve the final password.

**Concept:**  
Final validation.

**Approach:**  
Used knowledge from previous levels to locate and read the required file.

**Why it works:**  
The final level tests overall understanding rather than introducing new concepts.

**Key Takeaway:**  
Consistency and fundamentals matter more than complexity.

---

## Level 34

**Goal:**  
Completion of Bandit.

**Concept:**  
Wrap-up.

**Approach:**  
Successfully accessed the final level and verified completion.

**Why it works:**  
All previous skills contribute to reaching this point.

**Key Takeaway:**  
Progress comes from stacking small skills over time.

---

## Overall Takeaways (Level 27–34)

- Data can exist in version control history, not just files  
- Always check branches, tags, and commits  
- Instructions often contain the solution if read carefully  
- Simple solutions are often hidden behind overthinking  
- Consistency beats complexity
