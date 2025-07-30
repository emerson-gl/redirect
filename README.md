This was a first attempt at hosting a redirect file for use with a Prolific survey.

I quickly switched to https://app.netlify.com/ to host these simple redirect websites. Login is via my GitHub credentials if anyone ever needs to access the documents.

The reason for the redirect is Google Forms doesn't allow parsing the URL parameters passed by Prolific to automatically fill in the Prolific Paricipant ID in the form. It has to be passed to a Google URL via:

`https://docs.google.com/forms/d/e/1FAIpQLScLnWbWM0VD_ZlfVyS0_F97As53iCh4dg4nYKn4hHjOQOGmDQ/viewform?entry.########=${encodeURIComponent(pid)}`

...where ######## is the Google Forms prefill entry ID.
