# Manage-Authorization

<h1>Scenario</h1>
  
In this scenario, you must examine and manage the permissions on the files in the /home/researcher2/projects directory for the researcher2 user.

The researcher2 user is part of the research_team group.

You must check the permissions for all files in the directory, including any hidden files, to make sure that permissions align with the authorization that should be given. When it doesn't, you must change the permissions.

Here’s how you’ll do this task: First, you’ll check the user and group permissions for all files in the projects directory. Next, you’ll check whether any files have incorrect permissions and change the permissions as needed. Finally, you’ll check the permissions of the /home/researcher2/projects/drafts directory and modify these permissions to remove any unauthorized access.

<h1>Task 1. Check file and directory details</h1>

In this task, you must explore the permissions of the projects directory and the files it contains. The lab starts with /home/researcher2 as the current working directory. This is because you're changing permissions for files and directories belonging to the researcher2 user.

1. Navigate to the projects directory.

  ![image](https://github.com/user-attachments/assets/16e86902-26af-4f88-91b1-551f2eff0417)
 
2. List the contents and permissions of the projects directory.

![image](https://github.com/user-attachments/assets/e473d4fd-5abf-4c32-aa9f-00f8b4d26897)

3. Check whether any hidden files exist in the projects directory.

![image](https://github.com/user-attachments/assets/c87e7392-14b8-4318-905c-0ff6c57dca34)


<h1>Task 2. Change file permissions</h1>

In this task, you must determine whether any files have incorrect permissions and then change the permissions as needed. This action will remove unauthorized access and strengthen security on the system.

None of the files should allow the other users to write to files.

1. Check whether any files in the projects directory have write permissions for the owner type of other.

   ![image](https://github.com/user-attachments/assets/18309486-3b08-4df0-ab9d-1d148df32e91)

   2. Change the permissions of the file identified in the previous step so that the owner type of other doesn’t have write permissions.

![image](https://github.com/user-attachments/assets/34696ff0-fb50-486a-88df-01b4addbcff8)

3. The file project_m.txt is a restricted file and should not be readable or writable by the group or other; only the user should have these permissions on this file. List the contents and permissions of the current directory and check if the group has read or write permissions.

![image](https://github.com/user-attachments/assets/0f1c630a-6f34-493e-ba84-dfb467361456)

4. Use the chmod command to change permissions of the project_m.txt file so that the group doesn’t have read or write permissions.


![image](https://github.com/user-attachments/assets/cc761c19-419c-47d7-a99c-ce7d3c2bbb4d)


<h1>Task 3. Change file permissions on a hidden file</h1>

In this task, you must determine if a hidden file has incorrect permissions and then change the permissions as needed. This action will further remove unauthorized access and strengthen security on the system.

The file .project_x.txt is a hidden file that has been archived and should not be written to by anyone. (The user and group should still be able to read this file.)

1. Check the permissions of the hidden file .project_x.txt and answer the question that follows.


![image](https://github.com/user-attachments/assets/b04e638c-f201-44d3-93f6-0b9bfd31c36a)

2. Change the permissions of the file .project_x.txt so that both the user and the group can read, but not write to, the file.


![image](https://github.com/user-attachments/assets/efe701f9-2c77-4e4b-b964-60373c3cc767)



