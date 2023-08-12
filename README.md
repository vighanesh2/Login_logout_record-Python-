![image](https://github.com/vighanesh2/Login_logout_record-Python-/assets/103332350/d4154974-28d4-4d2c-a83a-d5b0d95bc43b)# Login_logout_record-Python-
Login/Logout Event Tracker
This Python script is designed to process login and logout events and generate a report of users' activity on different machines. It maintains a record of user login and logout events for various machines and produces a summary report of users' activity on each machine.


Features
Process login and logout events for multiple machines and users.
Generate a summary report of users' activity on each machine.
How to Use
Modify the events list in the script to include your own login and logout events.
Run the script using a Python interpreter: python login_logout_tracker.py.
Code Description
The script consists of three main functions:

get_event_date(event)
This function is used to extract the event date from an event object.

current_users(events)
This function processes the list of events and tracks the current users on each machine. It returns a dictionary where each machine maps to a set of users currently logged in.

generate_report(machines)
This function takes the dictionary of machines and their associated users and generates a report by printing out the users' activity on each machine.

Event Class
The Event class defines the structure of an event object. It has the following attributes:

event_date: The date and time of the event.
event_type: The type of event (login/logout).
machine_name: The name of the machine.
user: The user associated with the event.
Example Events
The script includes an example list of events. You can replace these events with your own data.

python
Copy code
events = [
    Event('2020-01-21 12:45:56', 'login', 'myworkstation.local', 'jordan'),
    Event('2020-01-22 15:53:42', 'logout', 'webserver.local', 'jordan'),
    # ... (other events)
]
