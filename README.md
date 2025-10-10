TOPIC:EMAIL REMAINDER SYSTEM

#Main Goal
The primary goal of this project is to provide a lightweight, front-end-only reminder system where users can input an email address, a subject, and a specific date and time to be reminded. Although it does not send actual emails, it simulates the process of managing scheduled reminders in a user-friendly interface and highlights overdue tasks.

#Features
1.Add a new reminder by entering email, subject, date, and time.
2.Reminders are displayed in a list format under the form.
3.Overdue reminders are visually highlighted in a different color.
4.Users can delete reminders with a simple "X" button.
5.All reminders are saved in localStorage so they persist even after page reloads.
6.The reminder list auto-refreshes every 10 seconds to update the overdue status.

#Technologies Used
1.HTML5 for structuring the page.
2.CSS3 for styling the form and reminder list.
3.Vanilla JavaScript for handling the logic of adding, deleting, and rendering reminders.
4.LocalStorage to persist reminders in the browser without any backend or database.

#How It Works
When the user submits the form by entering an email, a subject, a date, and a time, a new reminder object is created. This object includes a unique ID, the entered details, and a combined timestamp (dateTime) based on the date and time fields.
This object is pushed into a reminders array, which is stored in the browser's localStorage to persist the data.
Each reminder is then displayed in a list. The application checks whether the reminder's date and time are in the past; if so, it marks the reminder as "overdue" using a different background color.
Users can delete a reminder by clicking the "X" button associated with each entry. The reminder list refreshes automatically every 10 seconds to check if any reminders have become overdue since the last render.
