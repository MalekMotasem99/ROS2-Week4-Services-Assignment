Building a Task Management System Using ROS2 Services – Week 4 Assignment

Name : Malek Humoudeh  
Course : ROS2  

Description :  
This repository contains my Week 4 assignment, where I built a complete Task Management System using ROS2 Custom Services.  
The system allows creating tasks, assigning priorities, executing them in order, and checking their status.

• Custom Service Definitions :

1) AddTask.srv  
   - Request: task_type, priority, parameters  
   - Response: task_id, success, message  

2) GetTaskStatus.srv  
   - Request: task_id  
   - Response: status  

• System Implementation :

The system is built using three main nodes:

• Task Server  
  - Receives AddTask & GetTaskStatus requests  
  - Assigns IDs and stores tasks  
  - Communicates with the executor  

• Task Executor  
  - Uses a Priority Queue  
  - Executes tasks based on priority  
  - Updates task status  

• Task Client  
  - Sends multiple AddTask requests  
  - Queries task status  

Video File : assignment-4-malek_e2pmQu3S.mp4  
