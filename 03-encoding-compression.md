# Encoding & Compression (Level 11–15)

This section introduces data transformation techniques like encoding, rotation ciphers, and multiple layers of compression.  
The main challenge here is not the commands themselves, but recognizing patterns and applying the correct sequence of steps.

---

## Level 11

**Goal:**  
Decode a text that has been rotated (Caesar cipher).

**Concept:**  
ROT13 encoding.

**Approach:**  
Used `tr` to rotate characters:
`tr 'A-Za-z' 'N-ZA-Mn-za-m'`

**Why it works:**  
ROT13 shifts each letter by 13 positions in the alphabet. Applying the transformation restores the original text.

**Key Takeaway:**  
Simple encoding techniques can hide data in plain sight.

---

## Level 12

**Goal:**  
Extract useful data from a hex dump.

**Concept:**  
Hexadecimal representation of data.

**Approach:**  
Used `xxd -r` to reverse the hex dump back into its original binary format.

**Why it works:**  
Hex dumps represent binary data in readable form. Reversing it reconstructs the original file.

**Key Takeaway:**  
Data can be transformed into different formats—understanding how to reverse it is crucial.

---

## Level 13

**Goal:**  
Log into the next level using a private SSH key.

**Concept:**  
SSH key-based authentication.

**Approach:**  
Used:
`ssh -i private_key_file user@host`

**Why it works:**  
Instead of passwords, SSH can authenticate users using key pairs. The private key grants access if it matches the server’s public key.

**Key Takeaway:**  
Authentication isn’t always password-based—keys are often used in real systems.

---

## Level 14

**Goal:**  
Retrieve a password by connecting to a service on a specific port.

**Concept:**  
Network communication via local ports.

**Approach:**  
Used `nc` (netcat) to connect to the given port and send the required input.

**Why it works:**  
Netcat allows direct interaction with services over TCP/UDP, making it useful for testing and data retrieval.

**Key Takeaway:**  
Services running on ports can expose sensitive information if accessed correctly.

---

## Level 15

**Goal:**  
Handle multiple layers of compressed data.

**Concept:**  
Nested compression formats.

**Approach:**  
Repeatedly identified file types using `file`, then used appropriate tools like:
- `gzip`
- `bzip2`
- `tar`

to extract data step by step.

**Why it works:**  
Each compression layer must be handled with the correct tool. Identifying the format is key to choosing the right command.

**Key Takeaway:**  
Complex problems are often just multiple simple steps stacked together.

---

## Overall Takeaways (Level 11–15)

- Encoding and compression are common ways to hide data  
- Pattern recognition is more important than memorizing commands  
- Always identify data format before acting  
- Break problems into smaller steps instead of rushing
