# FME Workflow Runner


Each dataset on the ChattaData portal is refreshed nightly by a workflow. That workflow is itself started by yet another workflow that keeps a log of if the process succeeded or failed.

In the folder of each dataset there's two .fmw files used for updating a dataset. One is the FME file used to update the actual data, and should have a descriptive name of what its updating. The other will be called runner_v3.fmw. This is the file that gets called to run by PTFB. 

### The EXE
To get the line needed for PTFB run the runner and take a look at the very top of the Translation Log window. The text directly under "Command-line to run this workspace" is the text needed. Copy and paste this into the editing tab of PTFB. 

### The Job Log
Each time a runner is used it sends a log of what happened to Socrata. There are two attributes that are specific to the workflow. They can both be found in the second transformer which is named AttributeCreator. Double click this transformer to edit. The job name is what will appear in the workflow log. The Path to fmw file is the file that will be ran by the runner.
