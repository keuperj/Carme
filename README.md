# Carme

## HPC meets interactive Data Science and Machine Learning 
Carme (/ˈkɑːrmiː/ KAR-mee; Greek: Κάρμη) is a Jupiter moon, also giving the name for a Cluster of Jupiter moons (the carme group).

Or in our case:

an open source frame work to mange resources for multiple users running Jupyter notebooks on a 
Cluster of (GPU) compute nodes.

## Carme core idea:

Combine established open source ML and DS tools with HPC back-ends
* Use containers -> (for now) Docker 
* Use Jupyter Notebooks as main web based GUI-Frontend
* All web front-end (OS independent, no installation on user side needed)   
* Use HPC job management and scheduler -> SLURM
* Use HPC data I/O technology -> ITWM’s BeeGFS  
* Use HPC maintenance and monitoring tools 

## Key Features

* Open source
 * Carme uses only opensource components that allow commercial usage
 * Carme is open source, allowing commercial usage  
* User Management 
 * User quotas (GPU time, priority, GPUs per job, jobs per time, Disk quota)
 * Different User Roles (Quotas, right to add containers) 
* Container Management
 * Container store (user selects from predefined containers)
 * Adding of user defined containers
* Scheduler
  * Resource reservation (calender)
  * Job queues for large jobs and instant interactive access for small jobs   
* Data Management and I/O
  * Redundant, global file system (BeeGFS), mounts into container
  * Temporary job FS on local SSDs for max performance (BeeOND) 
* Web-Interface
 * HTTPS and SSH (if allowed) access via proxy 
 * Web front-end (management and IDE)   
 
## Comming soon...
The Carme prototype (alpha) is currently up and running - we are working towards the first beta release to be presented at ISC 18 (mid June)

## Who is behind Carme?
Carme is currently developed at the machine learning group of the Fraunhofer Competence Center HPC -> http://itwm.fraunhofer.de/ml 
