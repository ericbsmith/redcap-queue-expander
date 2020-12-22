# REDCap Queue Expander
This REDCap external module removes the need for a user to click the "view all" link to expand the survey queue.

## Author 
Eric Smith, Frontier Science Scotland Ltd

## How it Works
Queue Expander works by injecting JavaScript into the redcap_every_page_top & redcap_survey_complete hooks.  The code checks that the current page is a Survey Queue, shows any hidden surveys and removes the "view all" link and table row.

### Before Queue Expander
When a survey queue has more than 6 completed surveys the queue is collapsed and the user must click "view all" to expand the queue. This is an unneccesary step in projects which rely on multiple surveys.

### After Queue Expander
The survey queue is automatically expanded and the user does not require an extra mouse click.

### Future Functioanlity
At present the user will still require to click "view all" on the Surevy Queue which is displayed via the window overlay. It would be useful to expand that queue in the future.

## Version History
v1.0.0 -- initial version
