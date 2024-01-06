+----------------+       +-------------------+       +------------------+       +----------------+       +-------------------+
|   Faculty      |       |   Class/Lab       |       |    Timetable     |       |    Subject     |       |   Department      |
+----------------+       +-------------------+       +------------------+       +----------------+       +-------------------+
| faculty_id (PK)| 1---n | class_lab_id (PK) | 1---n | timetable_id (PK)|       | subject_id (PK)| 1---n | department_id (PK)|
| name           |       | name              |       | day              | 1---n | name           |       | name              |
| title          |       | capacity          |       | time_slot        |       |                |       |                   |
| department_id (FK)|    | department_id (FK)|       | faculty_id (FK)  |       |                |       |                   |
| ...            |       | ...               |       +------------------+       +----------------+       +-------------------+
+----------------+       +-------------------+                                                  
                                 |                                                          
                                 |                                                          
                                 v                                                          
                           +-------------+                                                  
                           |    Admin    |                                                  
                           +-------------+                                                  
                           | admin_id (PK)|                                                  
                           | username    |                                                  
                           | password    |                                                  
                           +-------------+                                                  

