# DOECE Alumni Portal
### Languages, Frameworks:
Python, Django, PostGreSQL
### Features:<br>
- View Yearbook and change own's details for students (No log in protection...)
- Complete Database, and list views and edit views implemented
- Solid django admin app
- Back end hosting and backup concepts implemented 
- Signup and Login feature for students using email/password credentials 
- An institute level access system
    * Such users can view and edit student data like in admin, but through a django app that we created.
    * Features in the app:
        - A versatile/robust filter based on categories(single,multiple)
        - Select, view and edit student data

-----------------------------------------------------------------------------------------------------------------------

#### Procedure to run this project on your local machine:<br>
- Create a group Students
- Create a group Institutes
   - Create a user and add it to the institute group
   - Create an entry in the Institutes model
   - Use a user in Institutes group in this entry's user field
- &lt;host&gt;/institute is the address to access institute facilities
   

### Project Details
Main django app- DOECEAlumniStudent<br>
Django app for records - records<br>
pip install -r requirements.txt<br>
Database settings are in DOECEAlumniStudent/settings.py, towards the end.

Development:<br>
In settings.py, at the end, 
1) comment out the lines between 
    "#PRODUCTION(Manaslu Server) START"
    and
    "#PRODUCTION(Manaslu Server) END"
2) uncomment out the lines between 
    "#DEVELOPMENT START"
    and
    "#DEVELOPMENT END"
    
Production:<br>
The opposite of the above

backup_script.sh backups the PostGreSQL database as well as the media files.
More details in server_notes/ directory.

