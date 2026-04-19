# File Discovery & Data Inspection (Level 6–10)

This section focuses on identifying the correct files, understanding file types, and extracting useful information from data.  
The difficulty increases slightly here—not because commands are complex, but because observation matters more.

---

## Level 6

**Goal:**  
Find a file with specific conditions (size, permissions, ownership).

**Concept:**  
Advanced file searching using filters.

**Approach:**  
Used the `find` command with parameters like:
- file size  
- user/group ownership  
- permissions  

to narrow down results and locate the correct file.

**Why it works:**  
`find` allows filtering based on multiple attributes, making it much faster than manually checking files.

**Key Takeaway:**  
Precise searching saves time—manual exploration doesn’t scale.

---

## Level 7

**Goal:**  
Locate a specific word inside a file.

**Concept:**  
Searching inside file content.

**Approach:**  
Used `grep` to search for a specific keyword within the file.

**Why it works:**  
`grep` scans file content and returns lines that match a given pattern.

**Key Takeaway:**  
Sometimes the data you need is inside files, not in filenames.

---

## Level 8

**Goal:**  
Find a unique line among repeated entries.

**Concept:**  
Sorting and filtering duplicate data.

**Approach:**  
Used:
- `sort` to organize data  
- `uniq` to filter unique lines  

Often combined like:
`sort file | uniq -u`

**Why it works:**  
`uniq` only works on sorted input, so sorting ensures duplicates are grouped together.

**Key Takeaway:**  
Command chaining is powerful—simple tools become effective when combined.

---

## Level 9

**Goal:**  
Extract readable information from a binary file.

**Concept:**  
Reading non-text files.

**Approach:**  
Used `strings` to extract human-readable text from the file.

**Why it works:**  
Binary files may contain embedded readable strings, which `strings` can reveal.

**Key Takeaway:**  
Even if a file looks unreadable, it may still contain useful information.

---

## Level 10

**Goal:**  
Decode encoded data.

**Concept:**  
Base64 encoding.

**Approach:**  
Used:
`base64 -d`
to decode the file contents.

**Why it works:**  
Base64 encodes data into readable characters, but it must be decoded to retrieve the original content.

**Key Takeaway:**  
Not all data is directly usable—recognizing encoding patterns is important.

---

## Overall Takeaways (Level 6–10)

- Searching smartly is better than searching blindly  
- Data inside files matters as much as filenames  
- Combining commands unlocks real power  
- Not all data is readable at first glance
