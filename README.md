# ConfigMgrWizardReplacement
Simple FrontEnd for SCCM Task Sequence.
<br>
With this we can replace the Wizard when starting a Task Sequence from PXE.
<br>
It works by placing a JSON file at a web server that an HTA is reading.
<br>
This will set an override TS advertisement id so that the default Wizard is skipped.
<br>

Simple video of how it looks like -> https://youtu.be/EXNGwAAhNiY

## Install

1. Create a simple web app in IIS.
2. Copy the content from WebApp to this folder.
3. Change variable jsonUrl in FrontEnd.hta

### Bootimage
3. Prestart commnad: mshta.exe "x:\sms\pkg\SMS10000\FrontEnd.hta"
4. Source Directory, point to the folder with "FrontEnd.hta",css,fonts and scripts.
5. Remember to add Winpe-HTA