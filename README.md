# Nile Ops Workstation — Linux CLI & Administration Assessment

## Overview
This repository contains the complete documentation and execution proof for the **Nile Ops Workstation Lab** executed on **Kali Linux**. 

The assessment simulates a junior Linux administrator onboarding scenario under a strict **Terminal-Only constraint** (no GUI tools, VS Code, or prohibited commands like `mv`). All file creation, workspace tree architecture, backup mechanisms, cleanup operations, and audit logging were completed using Linux standard shell utilities.

---

## Technical Objectives & Tasks Breakdown

### Part A: System Reconnaissance & Filesystem Hierarchy
- Executed core inspection tools (`pwd`, `cd /`, `ls -la`) to map out system paths[cite: 4, 5].
- Analyzed essential system directories (`/etc`, `/home`, `/var/log`, `/bin`, `/tmp`)[cite: 4, 5].
- Extracted system identification details from `/etc/hostname` and `/etc/os-release` (`Kali GNU/Linux Rolling`)[cite: 4, 5].
- Managed fast path navigation techniques using `cd -` and inspected hidden directory entries sorted by timestamp (`ls -lt`)[cite: 4, 5].

### Part B: Workspace Architecture Setup (`nile_ops`)
Recreated a multi-tier project tree under `~/nile_ops` meeting strict command constraints[cite: 4]:
- Built complete directory hierarchy (`admin/`, `.secrets/`, `policies/`, `projects/`, `scratch/`, etc.) using efficient `mkdir -p` flags[cite: 4, 5].
- Provisioned baseline system files (`contacts.txt`, `vault.note`, `main.txt`, `utils.txt`, `.hidden_note`, etc.) using optimized `touch` invocations[cite: 4, 5].
- Analyzed inode timestamp update behaviors upon re-touching existing targets[cite: 4].

### Part C: Content Authoring & Stream Redirection
- **Interactive Editing:** Used `nano` editor without mouse interaction to format administrative user profiles (`contacts.txt`)[cite: 4, 5].
- **Stream Redirection:** Utilized standard output redirection (`>`) to populate entry-point parameters and append redirection (`>>`) to insert metadata into `main.txt`[cite: 4, 5].
- **File Concatenation:** Merged multiple source documents (`main.txt`, `utils.txt`, `readme.txt`) into a unified release document (`alpha_bundle.txt`)[cite: 4, 5].

### Part D: Backup & Duplication Procedures (`cp`)
- Executed single-file renamed copies (`cp contacts.txt backup/contacts_backup.txt`)[cite: 4, 5].
- Handled directory-tree duplication using recursive copy flags (`cp -r`)[cite: 4, 5].
- Performed multi-file single-command batch transfers and verified hidden structural items (`.secrets`)[cite: 4, 5].

### Part E: Destruction & Clean-up Operations
- Tested directory deletion safety constraints (`rmdir` failure on non-empty directories vs `rm -r`)[cite: 4, 5].
- Executed interactive deletion prompts (`rm -ri`) to prevent data loss[cite: 4, 5].
- Performed a Disaster Recovery drill restoring `contacts.txt` from secondary backup storage[cite: 4, 5].

### Part F: Submission Assembly & Audit Trail
- Generated an immutable audit trail (`commands.log`)[cite: 4, 5].
- Captured the final directory tree state (`final_tree.txt`)[cite: 4, 5].
- Assembled the comprehensive evaluation submission (`submission.txt`) via a single concatenated stream[cite: 4, 5].

### Bonus Challenges Solved
- Handled filenames containing spaces via double quoting (`"team notes.txt"`)[cite: 4, 5].
- Traversed workspace structures using strict relative path navigation (`../../backup`)[cite: 4, 5].

---

## Project Structure
- `linux_practical.pdf`: Terminal screenshot evidence and step-by-step logs.
- `README.md`: Technical summary and execution overview.

## Environment Details
- **OS:** Kali Linux (GNU/Linux Rolling)[cite: 5]
- **Shell:** Zsh / Bash CLI[cite: 5]
