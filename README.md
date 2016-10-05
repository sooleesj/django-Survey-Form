# django-Survey-Form

This is one of assignment from Coding Dojo. Using Django, building a simple survey form web app.

### Description

For any web app, it’s critical that you understand how a **form** can be submitted and how **POST**, as well as **session**, data work. As you build the app described below, make sure you feel very comfortable with how information can be relayed between a **form** and controller/view (found in **views.py** currently), and how **session** and **POST** data are being handled.

### Task
- Do not have a single URL handle BOTH the **POST** submission as well as **render** the view file.
  - For example, the **form** that’s rendered from http://localhost should be submitted not to **/result** but to **/surveys/process**. The method that handles **/survey/process** should do all the logic, process **POST** data, manipulate session data and redirect to another URL, say **/result**.
  - The reason we have a method to handle POST/session and another method to handle the view file is because it makes reading your code much easier.
  - Also, if the same URL handled both **POST** and the rendering of the view when you reload that page, it would resubmit the form data. This is not a good thing.
