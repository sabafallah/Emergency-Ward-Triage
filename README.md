# Emergency-Ward-Triage
A Java based program made as a project for one of my second year courses.

completed the implementation of a system to triage patients in a hospital emergency ward. Patients are triaged according to both medical priority and wait time. Priorities are positive integers; the highest priority is 1. Normally patients are seen in priority order. However, if there are patients who have waited longer than a specified time (maxWait), they are seen first, in order of their arrival. 
To achieve this, the system I used two location-aware priority queues implemented with min heaps: one based on medical priority and the other on arrival time. The heaps use ArrayLists to store the underlying binary trees.
When a patient is removed from one queue they are also removed from the other. Location-aware priority queues allow us to do this efficiently.

