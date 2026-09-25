# Homework 2 — Part 2 Submission

Student name: Kadidja Traore

GitHub username: Mouhadidja2

## 1. Git Command Observations

| Command or workflow | What did you observe? | What was the user trying to accomplish? | What problem or risk did it address? |

1. git status
The first command I chose to observe is git status. I observed that this command displays the current state of the repository, showing which files have uncommitted changes. The user was trying to accomplish seeing if any changes had been made and checking what was currently in the staging area. This addresses the risk of accidentally committing the wrong files or forgetting to stage an important file before making a commit.
2. git diff
The second command is git diff. I observed that it shows a comparison of the original file versus what was edited, usually highlighting the additions and deletions in green and red. The user was trying to see the exact changes they made to their file before moving it to the staging area. This command addresses the problem of introducing unintended code changes by forcing the user to review their raw edits.
3. git add
The third command I selected is git add. I observed that entering this command moves the newly edited and verified file directly into the staging area. The user was trying to accomplish getting their specific changes ready to be officially committed to the repository. This addresses the risk of grouping unrelated changes together by letting the user selectively choose exactly which files to stage.
4. git diff --staged
The final command I observed is git diff --staged. I observed that this outputs a line by line check exclusively for the files that have already been staged. The user was trying to accomplish a final review of the exact modifications that are queued up for the next commit. This addresses the risk of committing incomplete or broken code by acting as a final safeguard right before the commit is made.


## 2. User Needs

#### UN-GIT-01 —  View line edits
A student programmer needs a way to review the exact lines of code they just changed because they want to catch typos or errors before finalizing their work. 

#### UN-GIT-02 — View state of repository
A programming teacher needs a way to identify the state of the program they are  teaching because they would want to make sure there is no error or unfinished work in their program.

#### UN-GIT-03 — Value of drafting
A programmer needs a way to save a draft of their changes because they want to review the code one last time before permanently submitting it.

#### UN-GIT-04 — Value of reviewing the drafts
A programmer needs a way to save a draft of their changes because they want to review the code one last time before permanently submitting it.



## 3. User Requirements

| ID and short title | User requirement | Source user need | Rationale |

UR-GIT-01:  A student programmer shall be able to view a line by line change and comparison before saving their work to the drafts(staging area).

UR-GIT-02: A programming teacher shall be able to identify the state of the program they are using before continuing with any other changes with the file.

UR-GIT-03: A programmer shall be able to save a draft of their changes before  permanently submitting it.

UR-GIT-04: A programmer shall be able to see the changes and comparaisons made in the drafts (staging area)before  permanently submitting it.

| UR-GIT-01 View line edits |  A student programmer shall be able to view a line by line change and comparison before saving their work to the drafts | View program line edits   | to catch typos or errors before finalizing their work.  |

| UR-GIT-02 View state of repository | A programming teacher shall be able to identify the state of the program they are using before continuing with any other changes with the file. | View state of repository |to make sure there is no error or unfinished work in their program. |

| UR-GIT-03 Value of drafting | A programmer shall be able to save a draft of their changes before  permanently submitting it. |  Value of drafting | to review the code one last time before permanently submitting it.|

| UR-GIT-04 Value of reviewing draft edits|  A programmer shall be able to see the changes and comparaisons made in the drafts (staging area)before  permanently submitting it. |Value of reviewing draft edits|  to review the draft of the code one last time before permanently submitting it.|

