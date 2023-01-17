# System Overview

## User Experience

The purpose of this system is to be able to schedule and manage family appointments at the Clothes Closet via an interactive website. Usage of this system depends on the type of user, for which there are two:

### (1) Parent/Guardian Experience

It starts with the parent or guardian going to the website at https://clothes-closet.herokuapp.com/, entering in their contact information, entering in the students that are to come to the appointment (by Student ID), and then selecting an available appointment date and time. The available appointment times are determined by events on the Clothes Closet Google Calendar which are labeled as open, and are otherwise not during are already booked appointment.

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/14.png)

When the "Schedule Appointment" button is pressed, the system checks against our own internal list of eligible students, which were given to us by the counselor. If a student is not on our list, they will receive an error stating so:

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/15.png)

Otherwise, if everything is valid, the appointment will be scheduled:

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/16.png)

#### Appointment Notification

Not done yet!

The intention is for the parent/guardian to be notified 24-hour prior via text message if they gave a mobile phone number, and then also by email.

### (2) Administrator

#### Calendar Management

It starts with the Clothes Closet Goolge calendar, which consits of times that it is avialable for appointment as designated by events labeled as "Open":

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/17.png)

...and events that are the result of a family booking:

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/18.png)

Note that none of the appointment details are available outside of the Clothes Closet Calendar, and the administrator protected portion of the online system.

#### Login

Login is done via a Google Account at https://clothes-closet.herokuapp.com/login, meaning that we defer to Google's own authenitcation system, but then the user in question must be on our own explicit list of allowed admins.

#### Appointment Search

Once logged in the admin has the ability to search through all appoinments by date and/or name:

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/19.png)

#### Appointment Printing

As during the appointment personal has to keep track of what each student took and adhere to certain limits, clicking on the "Print" button next to an apppointment brings up a version of the current form in use:

![01](/Users/john.valentino/workspaces/personal/clothes-closet-rest/wiki/20.png)

#### Appointment Selection

Pressing the "Select" button next to an appointment will bring up the data entry screen:

![01](./wiki/21.png)

This is where additonal people can be added to the appointment, quantities can be entered or updated, and the appointment can also be cancelled.

#### Settings Update

This refers to the settings by gender that are used to designate the quantities that one can take.

TBD: A user experience does not currently exist for this so its data must be entered manually by John Valentino directly into its database.

#### Student ID Upload

This refers to taking a spreadsheet as issued by the district and uploading it into our system.

TBD: A user experience does not currently exist for this so its data must be entered manually by John Valentino directly into its database.