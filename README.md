Copy Data disk from one Azure virtual machine to another
========================================================

            

Want to know about innovative and interesting ideas in Azure and automation? Check out my blog: https://manjunathrao.com/


 


Consider a case where you have configured an Azure virtual machine that hosts applications and you have saved an application data in multiple data disks. Now you want to create multiple virtual machines or copy all those data disks to other virtual machines.


Use the below code to copy data disks from one virtual machine to another machine. Source and destination virtual machines must be in same Resource Group.


 


1. Create a temporary Snapshot of Data disk


2. Create Managed disk from Snapshot created in Step 1


3. Attach the Managed disk (created from Step 2) to the destination Azure virtual machine


4. Update the destination Azure virtual machine with the new Managed disks


5. Delete the temporary Snapshots


 


 

 


 


        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
