# REDCap Queue Expander
This REDCap external module removes the need for a user to click the "view all" link to expand the survey queue.

## Author 
Eric Smith, Frontier Science Scotland Ltd

## How it Works
Queue Expander works by injecting JavaScript into the redcap_every_page_top hook.  The code checks that the current page is a Survey Queue and then shows any hidden surveys.  It then removes the "View All" link and table row.

### Before Queue Expander
When a survey queue has more than 6 completed surveys the queue is collapsed and the user must click View All to expand the queue. This is an unneccesary step in projects which rely on multiple surveys.

### After Stealth Queue
The survey queue is automatically expanded and the user does require an extra mouse click.

## Version History
v1.0.0 -- initial version