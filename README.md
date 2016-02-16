# ConfigMgrWizardReplacement
Simple FrontEnd for SCCM Task Sequence.
<br>
With this we can replace the Wizard when starting a Task Sequence from PXE.
<br>
It works by placing a JSON file at a web server that an HTA is reading.
<br>
This will set an override TS advertisement id so that the default Wizard is skipped.

## Install

1. Create a simple web app in IIS.
2. Copy the content from WebApp to this folder.