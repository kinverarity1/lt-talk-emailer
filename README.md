# lt-talk-emailer

**The below is not yet implemented.**

This tool is a hosted web project which emails updates on LT Talk threads to you. Sign up an account with an email address and enter the Talk threads that you want to be kept updated on. You can opt for a daily digest or email-per-post.

## Implementation 

Every four hours a queue should be started to cycle through all the nominated Talk threads. For each thread it should parse and store all the messages, then cycle over the users for that thread and the most recent dispatch to that user, and add the new messages that need dispatching.

Then there needs to be scheduled tasks for actually sending the emails.

I might do this as a Google App Engine project, as the Datastore would be convenient and presumably authentication will be much simpler.
