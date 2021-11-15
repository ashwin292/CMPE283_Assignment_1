# CMPE283_Assignment_1
## Individual submission by **Ashwin Kumar**

**Steps Followed:**
1. I installed Ubuntu on my existing system.
2. Then opened the terminal and executed the command "**cat /proc/cpuinfo**" and checked "**vmx flags"** features.
3. The presence of "**vmx flags**" indicated that my system supports hardware assisted virtualization.
4. Downloaded **cmpe283-1.c** file and **make** file into a folder.
5. Opened **283-1.c** file in text editor and made the relevant changes for different MSR controls.
6. I referred Intel SDM manual and searched for the relevant bit positions for required MSR controls.
7. Created **capability_info** struct arrays for primary procbased, secondary procbased, vmexit and vmentry controls.
8. Updated function **detect_vmx_features** for new function calls to the **rdmsr** function for new created struct arrays.
9. Added Licence details at the end of file.
10. Opened terminal into the folder created in step 4.
11. run "**make**" command.
12. The above command creates **cmpe283-1.ko** file.
13. Load this **.ko** file into the kernel through command "**sudo insmod cmpe283-1.ko**".
14. Run "**dmesg**" command to view the output.
