# Basics & Navigation (Level 0–5)

This section focuses on understanding the Linux environment, navigating directories, and accessing files.  
The challenges are simple, but they build habits that are used in every later level.

---

## Level 0

**Goal:**  
Log into the Bandit server using SSH.

**Concept:**  
Remote access using SSH.

**Approach:**  
Used the `ssh` command with the provided username, host, and port to connect to the remote machine.

**Why it works:**  
SSH allows secure remote login to another system. It is a fundamental tool in both system administration and cybersecurity.

**Key Takeaway:**  
Knowing how to access a system remotely is the first step before doing anything else.

---

## Level 1

**Goal:**  
Read the password stored in a file.

**Concept:**  
Basic file reading.

**Approach:**  
Listed files using `ls`, then used `cat` to read the contents of the file.

**Why it works:**  
`cat` displays file contents directly in the terminal.

**Key Takeaway:**  
Understanding how to locate and read files is the most basic but essential skill.

---

## Level 2

**Goal:**  
Access a file with spaces in its name.

**Concept:**  
Handling filenames with spaces.

**Approach:**  
Used quotes `"file name"` or escape characters `file\ name` to correctly reference the file.

**Why it works:**  
The shell treats spaces as separators. Quoting or escaping ensures the filename is treated as a single argument.

**Key Takeaway:**  
Command-line input must be precise—formatting mistakes can break commands.

---

## Level 3

**Goal:**  
Find a hidden file in a directory.

**Concept:**  
Hidden files in Linux.

**Approach:**  
Used `ls -a` to list all files, including hidden ones starting with `.`

**Why it works:**  
By default, `ls` hides files that begin with a dot. The `-a` flag reveals them.

**Key Takeaway:**  
Important files may not be visible unless you explicitly look for them.

---

## Level 4

**Goal:**  
Identify the correct file among multiple files.

**Concept:**  
File types and readable content.

**Approach:**  
Used the `file` command to identify file types, then used `cat` or similar tools to read the correct file.

**Why it works:**  
`file` helps distinguish between binary and readable files.

**Key Takeaway:**  
Not all files are readable—understanding file types helps you focus on the right ones.

---

## Level 5

**Goal:**  
Locate a file with specific properties.

**Concept:**  
Searching files using conditions.

**Approach:**  
Used the `find` command with filters like size, type, and permissions to locate the correct file.

**Why it works:**  
`find` allows precise searching based on attributes instead of manually checking everything.

**Key Takeaway:**  
Automation beats manual searching—use tools to narrow down targets efficiently.

---

## Overall Takeaways (Level 0–5)

- Learn your environment before acting  
- Small command mistakes can break everything  
- Hidden or unexpected data is common  
- Efficiency comes from using the right tools, not more effort
