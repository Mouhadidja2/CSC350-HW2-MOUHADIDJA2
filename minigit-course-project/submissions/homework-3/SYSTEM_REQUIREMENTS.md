# Homework 3 Submission

Add the Homework 3 submission files here when the assignment is released.

## Approved UN/UR Baseline

User needs


ID                    Stakeholder need
UN-GIT-01
A student developer needs a way to start tracking a local project because it has no recorded history.
UN-GIT-02
A student developer needs to know which project files have changed because they may forget what they edited before recording a checkpoint.
UN-GIT-03
A student developer needs to inspect changed content before recording it because a file may contain unintended edits.
UN-GIT-04
A student developer needs to choose the file content to include in the next checkpoint because some current changes may still be unfinished.
UN-GIT-05
A student developer needs to record a meaningful checkpoint because they want to record an important project version and provide a descriptive label.
UN-GIT-06
A student developer needs to review earlier checkpoints because they want to understand how the project reached its current state.
UN-GIT-07
A student developer needs invalid commands to explain why they failed while preserving existing project files and recorded checkpoints.


User requirements


ID       User-visible capability                Need

UR-GIT-01
A student developer shall be able to initialize tracking in the current local project folder without removing existing project files.
                                           UN-GIT-01, UN-GIT-07
UR-GIT-02
A student developer shall be able to see whether project files are untracked, staged, changed after staging, modified, deleted, or clean.
                                                  UN-GIT-02
UR-GIT-03
A student developer shall be able to view differences between current working file content and the content selected for the next checkpoint.
                                                UN-GIT-03
UR-GIT-04
A student developer shall be able to view differences between content selected for the next checkpoint and the latest recorded checkpoint.
                                                UN-GIT-03
UR-GIT-05
A student developer shall be able to select the current content of one existing project file for the next checkpoint without selecting unrelated files.
                                                UN-GIT-04
UR-GIT-06
A student developer shall be able to create a checkpoint of selected content with a nonempty explanation while leaving later unselected edits in the working files.
                                               UN-GIT-05, UN-GIT-04
UR-GIT-07
A student developer shall be able to view recorded checkpoints from newest to oldest, including their identifier and explanation.
                                                    UN-GIT-06
UR-GIT-08
A student developer shall receive a useful error when a command is invalid, a requested file is unavailable, or a path is outside the allowed project files.
                                                       UN-GIT-07
UR-GIT-09
A student developer shall be able to retry an operation after a failure without losing ordinary project files or an already recorded checkpoint.
                                                           UN-GIT-07

## UR-to-UN Mapping

UR-GIT-01 → source UN ID(s): UN-GIT-01, UN-GIT-07
UR-GIT-02 → UN-GIT-02 (worked example)
UR-GIT-03 → source UN ID(s): UN-GIT-03
UR-GIT-04 → source UN ID(s): UN-GIT-03
UR-GIT-05 → source UN ID(s): UN-GIT-04
UR-GIT-06 → source UN ID(s): UN-GIT-05, UN-GIT-04
UR-GIT-07 → source UN ID(s): UN-GIT-06
UR-GIT-08 → source UN ID(s): UN-GIT-07
UR-GIT-09 → source UN ID(s): UN-GIT-07

## Functional System Requirements
SR-01 first init
SR-01 (source UR-GIT-01): Given an uninitialized project folder containing existing files, when the init command is used, MiniGit shall initialize project tracking without deleting the existing project files.
Check: Inspect the project folder to confirm a tracking area was created and the original files are still there.

SR-02 repeated init
SR-02 (source UR-GIT-01, UR-GIT-09): Given an already initialized project with tracked history, when the init command is used again, MiniGit shall leave the existing recorded checkpoints and project files untouched.
Check: Inspect the existing tracking folder to ensure previous data was not overwritten or destroyed.

SR-03 add one existing file
SR-03 (source UR-GIT-05): Given an initialized project with notes.txt containing ONE and plan.txt present, when add notes.txt is used, MiniGit shall stage a copy of notes.txt containing ONE without staging plan.txt.
Check: Inspect the stage to confirm notes.txt is present and plan.txt is not.

SR-04 add a missing file
SR-04 (source UR-GIT-08, UR-GIT-09): Given an initialized project where notes.txt is already staged as ONE, when add missing.txt is used for a file that does not exist, MiniGit shall output a useful error and preserve the currently staged notes.txt.
Check: Inspect the terminal for the error message and inspect the stage to ensure notes.txt is still ONE.

SR-05 status for one staged file
SR-05 (source UR-GIT-02): Given an initialized project where notes.txt has been successfully added to the stage, when the status command is used, MiniGit shall display notes.txt clearly under a "staged" category.
Check: Inspect the terminal output of the status command to see where notes.txt is listed.

SR-05 verify one existing file
SR-05 ()