# Day_32-Birthday-wisher-project
An automated birthday wisher that sends personalized emails to people on their birthdays.

The program checks if today matches any birthday in a dataset, selects a random birthday message, personalizes it, and sends it through email. The project combines automation, data handling, and real-world functionality.


## How the code works:
- The program gets today’s date using the datetime module
- It reads birthday data from a CSV file using pandas (Birthdays are stored in a    dictionary for easy lookup)
- If today matches a birthday:
    A random letter template is selected
    The [NAME] placeholder is replaced with the actual name
    A personalized email is generated
- The email is sent using smtplib:
    Connects to an SMTP server
    Logs in securely
    Sends the email with a subject and message


## What I learned:
- Sending emails with Python (smtplib)
- Connecting to SMTP servers
- Using .starttls() for secure communication
- Logging in and sending emails programmatically
- Working with dates (datetime) 📅:
    Getting the current date
    Extracting specific components (day, month, weekday)
    Comparing dates for automation
- Structuring data for efficient lookup
- Selecting random templates for dynamic output
- Triggering actions based on real-world conditions (e.g., birthdays)
- Combining multiple modules into one system
- Reusable patterns 🔁, This same logic can be adapted for:
    Weekly emails 
    Notifications
    Reminders, etc.
