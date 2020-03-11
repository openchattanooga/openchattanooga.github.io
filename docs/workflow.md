# Workflow Automation

## Workflow Schedular

### Activate Schedular
PTFB is the application used for scheduling workflows every night. PTFB needs to be set to "Watching" to run scheduled events. There's a very simple way to do this. Either minimize the window, or click the "Start Watching" button found at the bottom right of the PTFB window.
If you want to be sure it's active, hover over the PTFB icon in the system tray and you'll get the message "PTFB Pro is Enabled".

### Running Individual Workflows
Workflows are scheduled individually. This makes it possible to easily turn them off and on when needed. A check mark next to the workflow indicates it's active. The "Item Name" is the description of the scheduled event. To actually adjust the time a workflow runs double click on the scheduled event. Then go to the Triggers tab and click the change button for schedule. Always keep the schedule Title up to date with the actual scheduled time of the workflow. It really helps troubleshooting issues when everything is organized.

### Running the FME exe
Each workflow is started by running an exe from PTFB. You'll find that line under the Editing tab of a scheduled event. Double click the event to make changes to it. How to get that line is covered in the FME Workflow Runner section. 


## FME Workflow Runner

## Adding to Nightly Run


