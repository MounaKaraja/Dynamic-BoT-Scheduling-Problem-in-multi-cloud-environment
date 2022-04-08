This dataset is proposed for the budget-constrained Dynamic Bag-of-Tasks Scheduling Problem (DBoTSP) in heterogeneous multi-cloud environment.
It contains synthetic instances generated randomly.
The dataset folder contains : 
- Instance data files (Small size instance, Medium size instance and Big size Instance).
- Bag-of-Tasks (BoT) data files
- Cloud data files (cloud1, cloud2 and cloud3)


The bag-of-Tasks files are named as follows: BOTX_Y such that X designs the BoT number and the Y designs the number of tasks within a BoT. 
30 differents BoT are considered in our dataset.
The number of tasks within a BoT is ranging from 50 tasks (BOT01_50 file) to 1500 tasks (BOT30_1500 file) with an increment of 50 tasks.
The first line of each BoT file defines its budget limit. The BoT budget is ranging from 0.45$ to 4.1$.
The rest of the file defines tasks within a BoT in millions of instructions such that each line represents a task.
Each task in a BoT contains a different number of instructions assigned randomly (using a uniformly distributed random number) ranging from 1,000 to 30,000 million of instructions with an increment of 1,000 million of instructions.


3 different instances are generated randomly each containing 100 BoT with different sizes. 
- The “Small Size Instance” file is composed by BoT including 50 to 500 tasks and budget ranging from 0.45$ to 1.4$. 
- The “Medium Size Instance” file contains BoT including 550 to 1000 tasks and budget ranging from 1.55$ to 2.75$. 
- And the “Big Size Instance” file contains BoT including 1050 to 1500 tasks and budget ranging from 2.9$ to 4.1$. 
Each instance file is composed by 100 lines. Each line represents a BoT file.


In our dataset the dynamic batch scheduling mode is considered such that BoTs are first collected in the scheduler waiting queue and will be examined for scheduling at predefined times.
To this end, 10 scheduling points are considered ranging from 1 to 10 hours with one hour increments.  
In each instance file, besides the BoT file name, the scheduling point for each BoT is defined.

3 heterogeneous clouds are considered in our dataset.
- The cloud1 is composed by 8 Virtual Machines (VMs) with different performances.
- The cloud2 is composed by 16 VMs with different performances.
- The cloud3 is composed by 24 VMs with different performances.
Each cloud data file categorizes the cloud VMs according to the execution speed and the execution cost.
The VM execution speed is ranging from 250 to 1500 million of instructions per seconds (mips) with an increment of 250 mips. 
the VM execution cost is ranging from 0.1 to 1.1$ with 0.2$ increments. 

For any further information, please contact me at: mouna.karaja.isg@gmail.com