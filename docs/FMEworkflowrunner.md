# FME Workflow Runner

### Process
Each dataset on the ChattaData portal is refreshed nightly by a workflow. That workflow is itself started by yet another workflow that keeps a log of if the process succeeded or failed.

### The Runner
In the folder of each dataset there's two .fmw files used for updating a dataset. One is the FME file used to update the actual data, and should have a descriptive name of what its updating. The other will be called runner_v3.fmw. This is the file that gets called to run by PTFB. To get the line needed for PTFB run the runner and take a look at the very top of the Translation Log window. The text directly under "Command-line to run this workspace" is the text needed. Copy and paste this into the editing tab of PTFB. 
