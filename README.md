--------------------------------------------------
## GitHub Storage & Remote Configuration
--------------------------------------------------

# * GitHub Storage Limits *

## Individual File Limits
* **50 MB:** Git will start giving a warning message in the terminal.
* **100 MB Hard Limit:** GitHub completely blocks files larger than 100 MB via normal push.
* **Solution for large files:** Use `.gitignore` to skip them or setup `Git LFS` (Large File Storage).

## Repository & Push Limits
* **Per Repository Max:** Recommended size is under 1 GB (Hard warning at 5 GB).
* **Per Push Limit:** Maximum data size for a single `git push` batch is 2 GB.
* **Account Limit:** Unlimited public and private repositories can be created on a single account.

--------------------------------------------------

--------------------------------------------------
