# VirtualER
This is a repo for a project I worked on that allows patients to easily find wait times of nearby emergency rooms to meet their medical needs. The project consisted of both a full implementation of the product as well as a detailed requirements phase, diagrams, and project planning. The project was for a Software Architecture class, but our design, tools used, approach, and system was all original work from our 4 person team. I would have liked to spend more time consulting with healthcare workers in order to more closely meet the needs of the actual healthcare field rather than the project requirements that were outlined. I am confident that we met the requirements for the scope of our project, but I feel like the application would need some serious overhauls to be used in any sort of workplace. One thing that I believe is a bit of an oversight with this project is that many workplaces simply don't have the staff to support an app like this. It requires too much help from ER staff to run properly. It would likely be better as an app that gives recommendations to patients on whether they need to seek further medical attention simply because it would be more easily adopted.

## Main application features
- ER Receptionist view
    - patient queue
    - request queue for patients that want to enter the queue remotely
    - fill out patient information form for
- Doctor/Nurse view
    - patient queue only with ability to modify SOI and remove
- Patient view
    - fill out questionnaire
    - join ER queue
- Admin view (Add/modify ERs, add users, )
  - add/modify ERs
  - add/modify users
  - database restoration/backup
- General features
  - JSON file database requests done through API POST/PUT/GET requests
  - Each user type can only access their respective URL (patient can't view receptionist page)
  - Calculated wait times based on number of users and their conditions


## System description
#### **Medical Information System To Enhance Resources for Emergency Departments - Virtual ER**

**Problem:** Patients are often left wondering whether they need to visit the Emergency Room (ER) based on their condition, which leads to them becoming crowded and overloaded. The "Virtual ER" system will be designed to help with this situation.

**Main Idea:** People who feel that they need to visit an ER will be able to use Virtual ER to understand the current load of ERs in their area and determine whether they need to visit the ER or follow some other course of action. Their questionnaire results will decide whether they need to come to the ER. If they need to come to the ER, they will enter the treatment queue; otherwise, the system will direct the patient with their next steps.

**Details:** They will be able to sign up for or login to an account online and undergo a questionnaire to determine whether they really should visit the ER or potentially follow another course of action, like going to a regular primary care clinic, taking over-the-counter medication, or contacting the nurse/clinician hotline over the phone or Internet.

Patients whose conditions are deemed "critical" will be immediately notified to seek emergency attention via calling 911.

Patients who have taken the questionnaire and still need to visit the ER are added to the treatment queue through the system and will be notified to come to the ER when they are close to the front of the queue.

Patients who have taken the questionnaire and do not need to visit the ER will be provided with recommendations such as going to a regular primary care clinic, taking over-the-counter medication, or contacting the nurse/clinician hotline over the phone or Internet.

Patients who are unable to take the online questionnaire will be directed to come to an ER in person. 

Individual ERs will need to be connected to the web service and update the wait times in real-time.

Doctors should be able to view the queue of patients with scheduled appointments for their ER, as well as view the information relating to that patient obtained throughout the triaging process. 

Doctors should be able to view the criticality of the current patient based on their triaging and questionnaire results, with priority going to patients in a critical state.
