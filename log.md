# 100 Days Of Code - Log

### Day 1: October 5, 2020

**Today's Progress**: Added tags, removed status, due, next action, and categories. Redesigned the backdrop and show/edit page, and added JS functionality to make new/update functions much cleaner (no separate pages).

**Thoughts:** CSS is a pain to figure out, but everything else was pretty straightforward. Integrating AJAX is going to be the next main technical challenge.


### Day 2: October 6, 2020

**Today's Progress**: Set up a Docker container so I can do all my development on my computer in an environment instead of being stuck with Cloud9 and its memory/Internet issues.

**Thoughts**: This was pretty fun to set up, but I'm stuck on getting rails or node server to start with localhost through the docker container.

### Day 3: October 7, 2020

**Today's Progress**: Redesigned the dashboard layout to be more user-friendly. Figured out what I wanted on it, and added dummy text while I build tag and task controllers with AJAX.

**Thoughts**: Wasn't any big technical challenge, but it was nice to get a feel for what the dashboard should look like design-wise, and to see it in real life before I code it up.

### Day 4: October 8, 2020

**Today's Progress**: Completed the tagging and search setup, so now I can assign tags to all interests, and easily select by tag if I need to look for specific tags. Weaknesses is that there's no direct delete function and it's a little clumsy to enter new tags. But it's all there if you use it carefully.

**Thoughts**: This was pretty technically challenging to implement, but [this tutorial](https://www.youtube.com/watch?v=oPpigFAlLmE) on adding tags to posts via hashtags helped a lot. Had to learn some [Regex](https://regexr.com/), which was painful, but very rewarding once I figured it out. 

### Day 5: October 9, 2020

**Today's Progress**: Added the Task model, so now you can view upcoming tasks from the dashboard, CRUD tasks from the contact page, and view a list of all tasks in the Task page. Still needs some Ajax and refinement, but core functionality is there. Also added some Bootstrap icons.

**Thoughts**: Building the model/controller side of things was tricky, because each task needs to be connected to an interest and built on the interest's page. But once that was done, the view setup was complicated, but didn't require any new significant technical expertise.


### Day 6: October 11, 2020

**Today's Progress**: Completed the Task model (added "task completed" status, ability to delete tasks, FontAwesome clickable icons), and fixed some problems with the database and creating new interests that were causing problems. Shipped version 2 of the app to the cloud.

**Thoughts**: Finishing the Task model was pretty fun. But pushing to the cloud and fixing the Heroku DB issue was hellish. I need to start writing tests and create a separate test Heroku environment so I'm not always deploying straight to the cloud, so I can avoid these issues. Also, be very careful when adding new models or messing with the database in any way. In the future, if I make any significant DB changes, I should release a whole new version of the software, so it doesn't mess with the existing one.

### Day 7: October 12, 2020

**Today's Progress**: Moved dev environment from Cloud9 back to native Mac OS. Also set up Heroku Pipeline, so whenever I've finished a new segment, I can just push it to GitHub on master, and it will auto-deploy to staging, where I can test it, make sure it works, and then promote it to the production environment.

**Thoughts**: Heroku Pipeline is incredibly cool. Wish I could do continuous integration testing for free, but it's really unnecessary because I'm the only one pushing code, so I can just write good tests and test code before I push it to GitHub.

### Day 8: October 13, 2020

**Today's Progress**: Revised the navbar to include a dropdown menu + user gravatars, moved main nav elements to a set of tabs inside the application, and fixed the bug with contact info displaying incorrectly.

**Thoughts**: Still pretty enamoured with Heroku Pipeline. It saved me a lot of stress having an identical production environment I can push to. Wrangling HTML/CSS can be really frustrating, and I'm unsure if I prefer the new tabbed design, but we'll see how it goes.

### Day 9: October 14, 2020

**Today's Progress**: Moved tag filtering to a dedicated tab to clean up the Interest interface. Modified the Tag setup, so you can create tags individually instead of in a big tagger. Built delete and "remove from interest" operations, so you can quickly edit and delete tags from the main page and within the app.

**Thoughts**: Honestly, I am quite proud of how this part turned out. Was tricky to sort some of the pieces out, but it all came together quite well, and now the tags are much simpler to manipulate and work very well. Pretty happy with the outcome.

### Day 10: October 15, 2020

**Today's Progress**: Removed tabbed navigation and replaced it with a sidebar. Does the same thing, but a lot more aesthetically pleasing. Looks more like an actual app. Also redesigned the contact show page after the Highrise model and removed all modals in favour of drop-downs and collapses. Now it looks a lot cleaner and simpler (less crowded). And finally, I moved the "Add Interest" button to the navbar. Looks much better and is universally available there. At some point I'll try to move tasks there, but it means messing with the database, so that's tricky.

**Thoughts**: Quite happy with how this turned out. Even though it's all aesthetic changes, it makes a big difference in the professional look and feel of the app. Modifying the navbar was a big pain, but definitely worth it. Next up with minor changes would be the search feature, adding JS validation to the forms, and rebuilding the login/signup/edit user pages.