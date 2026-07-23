# Question 5

## Aim

To evaluate the recovery mechanisms available in the vi editor after a system crash and identify the most reliable recovery method.

## Recovery Mechanisms in vi

### 1. Swap File
A swap file is automatically created while editing a file in vi. It stores unsaved changes and allows recovery if the system or editor crashes.

**Recovery Command:**
```bash
vim -r filename
```

### 2. Undo History
Undo history allows recently made changes to be reversed during the current editing session. If persistent undo is enabled, it can also restore changes from previous sessions.

### 3. Registers
Registers temporarily store copied, deleted, or yanked text. They are useful for recovering specific pieces of text but cannot restore an entire unsaved file after a crash.

### 4. Backup Files
If backup is enabled, vi creates a backup copy of the original file (such as `filename~` or `filename.bak`). These files can be used to restore previous content if needed.

### 5. Auto-Recovery
When vi detects a swap file after an unexpected crash, it prompts the user to recover the unsaved work automatically.

**Recovery Command:**
```bash
vim -r filename
```

## Most Reliable Recovery Strategy

The most reliable recovery mechanism is the **swap file** using the command `vim -r filename`. It preserves the latest unsaved changes made before the crash and provides the highest chance of recovering recent work. After recovery, the file should be saved immediately, and backup files can be used as an additional safety measure if required.

## Conclusion

The vi editor provides multiple recovery mechanisms, including swap files, undo history, registers, backup files, and auto-recovery. Among these, the swap file recovery method is the most reliable because it restores the latest unsaved changes after a crash.
