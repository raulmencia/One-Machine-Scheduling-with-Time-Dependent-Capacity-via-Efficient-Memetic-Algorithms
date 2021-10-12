

One-Machine Scheduling with Time-Dependent Capacity via Efficient Memetic Algorithms


This repository contains the problem instances used in the experimental study as well 
as detailed results.


INSTANCES
---------

The instances are contained in the folder "instances". Each file represents one instance, 
named "i<n>_<MC>_<id>.txt", where <n> is the number of jobs, <MC> denotes the maximum 
capacity of the machine and <id> is the index of the instance, ranging from 1 to 10.

The format of these files is as follows:

 - The two first lines indicate the number of jobs, "NOP: <nop>", and the number of 
   capacity intervals of the machine, "NINT: <nint>".

 - The following <nint> lines correspond to the different capacity intervals, and contain 
   three values: "<start> <end> <capacity>". This means that the machine has a capacity of 
   <capacity> units in the interval [<start>, <end>).

 - Finally, the last <nop> lines describe the jobs. These are of the form "<i> <pi> <di>", 
   where <i> is the index of the job, <pi> is its processing time and <di> its due date.


DETAILED RESULTS
----------------

The file "results.txt" contains the results obtained by each method in the experimental 
study on each of the instances. 

It contains two columns for each method <m>, <m>_Best and <m>_Avg. The methods are MA_SCP, 
MA_iSCP, MA_SCP+, MA_CB, MA_ICP, MA_HYB and CPO.

For each instance, it shows the best and average total tardiness obtained over 30 runs.

