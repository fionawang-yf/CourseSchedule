# My Personal Project

## Course Scheduling Overview

This application provides some courses available for the user to schedule, 
tell user what time is the course and ask if want to add to schedule or not. 
Some courses might have time conflict, it will show an error message if adding
not successful. At the end, show the user's course schedule. 

The reason why I want to do this project of this topic is because choosing courses
and managing timetable is a major problem I struggle with every year in university, 
when it comes to time for course registration. Hope this program might help me and 
other students in the future. 


## User Stories
**Tasks user should able to do:**
- As a user, I want to add courses to my schedule
- As a user, I want to see my timetable
- As a user, I want to be able to delete course from my schedule
- As a user, I want to know if course conflicts or not
- As a user, I want to be able to save my schedule
- As a user, I want to be able to be able to load my schedule from file

## Phase 4: Task 2 
I have chosen the option to make my class robust and throws a checked exception. 
- the name and course are variables needed to use get method inside the Schedule class. 
- inside the *Schedule* class, the methods: addNewCourse, searchCourse, and removeCourse
  throws exceptions. 
- since *ScheduleReader* calls function inside the *Schedule* class, the parseSchedule 
  method also throws exceptions.
- for *ScheduleApp, AddListener, RemoveListener, LoadFile* inside the ui package, 
  they all catch exceptions and give the user some feedbacks about the exceptions caught. 

## Phase 4: Task 3
If I have more time, I would probably implement my *Schedule* class differently, 
instead of list, I might use hashmap to map the course name and time, but I did this 
implementation before we learned about hashmap. Although my UML diagram for this project
might seems complicated, but I don't think there is much refactoring I can do, most of
the arrows are because when doing UI swing design, it is necessary to create different
class for each button, or else, the "actionPerformed" method will be too long. I feel like
I could refactor more in the *SchedulePanel* class if I had more time. I think my cohesion 
is okay, but maybe I can reduce some coupling, but since ScheduleApp and SchedulePanel are
two different ways of interacting with user, there isn't much I can reduce. I think I did 
follow the Single Responsibility Principle, each class has its own function.  


