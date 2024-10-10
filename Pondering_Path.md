# Challenge Summary: Invoking the `pwn` Program

1. **Objective**: Invoke the `pwn` program using its absolute path to retrieve the flag.
   - The command format is: `/pwn`

2. **Steps**:
   - Open a terminal and type the command with the absolute path:
     ```bash
     hacker@paths~the-root:~$ /pwn
     BOOM!!!
     Here is your flag:
     pwn.college{YgI0FcmIC3MYX2SG1T4_pPhBe0U.dhzN5QDL1MzM1czW}
     hacker@paths~the-root:~$
     ```

3. **Explanation**: In this challenge, you are required to provide the absolute path to the `pwn` program. The root of the filesystem is represented by `/`, and since the `pwn` program is located directly in the root directory, the absolute path is simply `/pwn`. Executing this command will prompt the system to return the corresponding flag.
   
# Challenge Summary: Invoking the `run` Program

1. **Objective**: Invoke the `run` program located in the `/challenge` directory using its absolute path to retrieve the flag.
   - The command format is: `/challenge/run`

2. **Steps**:
   - Open a terminal and type the command with the absolute path:
     ```bash
     hacker@paths~program-and-absolute-paths:~$ /challenge/run
     Correct!!!
     /challenge/run is an absolute path! Here is your flag:
     pwn.college{M7hMMc2vclsBmhiq3oFKtqF8vOn.dVDN1QDL1MzM1czW}
     hacker@paths~program-and-absolute-paths:~$
     ```

3. **Explanation**: In this challenge, you need to execute the `run` program located in the `/challenge` directory. The absolute path to this program is `/challenge/run`. By invoking this command, you will receive the corresponding flag.

# Challenge Summary: Changing Directories to Invoke the `run` Program

1. **Objective**: Change the directory to a specific path and then invoke the `run` program located in the `/challenge` directory to retrieve the flag.

2. **Steps**:
   - First, navigate to the required directory using the `cd` command:
     ```bash
     hacker@dojo:~$ cd /path/to/specific/directory
     ```
   - Next, invoke the `run` program from that directory:
     ```bash
     hacker@dojo:/path/to/specific/directory$ /challenge/run
     ```

3. **Explanation**: The Linux filesystem contains numerous directories and files. The `cd` (change directory) command allows you to navigate between directories, affecting the "current working directory" of your shell. In this challenge, you must first change to the specified directory before executing the `/challenge/run` program. This process is essential for ensuring that the command runs successfully and returns the flag.

 ![image](https://github.com/user-attachments/assets/4e906912-f958-4721-8bd9-8783eb7b56fb)

 ![image](https://github.com/user-attachments/assets/93ddd0b2-9201-42d8-94b7-820d717546f9)
 ![image](https://github.com/user-attachments/assets/acb1029a-2984-4de9-a746-1117734fa739)

 # Challenge Summary: Invoking the `run` Program with a Relative Path

1. **Objective**: Use a relative path to invoke the `run` program located in the `/challenge` directory while having the current working directory set to `/`.

2. **Steps**:
   - First, ensure your current working directory is set to `/`:
     ```bash
     hacker@dojo:~$ cd /
     ```
   - Next, invoke the `run` program using the relative path:
     ```bash
     hacker@dojo:/$ challenge/run
     ```

3. **Explanation**: The relative path `challenge/run` works because the cwd is `/`. Since `/challenge/run` is located directly under the root, you only need to refer to it relatively as `challenge/run` without the `/`.
![image](https://github.com/user-attachments/assets/dcb4ce0b-7343-446e-a073-08b8327acb56)

# Challenge Summary: Using Explicit Relative Paths with `.`

1. **Objective**: Use the explicit relative path with `.` to invoke the `run` program located in the `/challenge` directory.

2. **Steps**:
   - Ensure the current working directory is set to `/`:
     ```bash
     hacker@dojo:~$ cd /
     ```
   - Invoke the `run` program using an explicit relative path that includes `.`:
     ```bash
     hacker@dojo:/$ ./challenge/run
     ```

3. **Explanation**: In this challenge, the `.` symbol is utilized in relative paths, representing the current directory. Paths such as `challenge`, `./challenge`, or `./././challenge` are all equivalent to the absolute path `/challenge` when the current working directory is set to `/`. Executing the command with the explicit relative path allows for the successful retrieval of the corresponding flag.

   ![image](https://github.com/user-attachments/assets/b61e38d3-760f-4952-a36e-c22285d32fba)


   # Challenge Summary: Explicitly Using `.` to Invoke Programs

1. **Objective**: Invoke the `run` program from the `/challenge` directory using an explicit relative path that includes `.`.

2. **Steps**:
   - Change to the `/challenge` directory:
     ```bash
     hacker@dojo:~$ cd /challenge
     ```
   - Invoke the `run` program using the explicit relative path:
     ```bash
     hacker@dojo:/challenge$ ./run
     ```

3. **Explanation**: In this challenge, invoking the `run` program directly using a naked path (e.g., `run`) will result in an error due to Linux not searching the current directory for commands by default. This safety measure prevents accidental execution of programs with the same name as core system utilities. To successfully execute the `run` program, the explicit relative path `./run` is used, indicating that the program should be executed from the current directory. This approach ensures proper invocation and allows for the retrieval of the corresponding flag.

   ![image](https://github.com/user-attachments/assets/a763f702-d920-46e9-b9b6-3a86eaa99f5d)


   # Challenge Summary: Using the Home Directory for Output

1. **Objective**: Invoke the `run` program located in `/challenge`, specifying an absolute path inside the home directory as an argument, with a constraint on the length of the path before expansion.

2. **Steps**:
   - Change to the home directory if not already there:
     ```bash
     hacker@dojo:~$ cd ~
     
   
     ```
   - Invoke the `run` program with the absolute path to the created file:
     ```bash
     hacker@dojo:~$ /challenge/run ~/s
     ```

3. **Explanation**: In this challenge, the `run` program requires an absolute path as an argument. The path must be located within the user's home directory (`/home/hacker`). Additionally, the length of the argument before expansion must be three characters or less. This is important because paths are expanded by Bash, and ensuring compliance with these constraints enables successful flag retrieval. The command effectively creates a copy of the flag in the specified file.

![image](https://github.com/user-attachments/assets/ed5658ae-9c2f-403c-8038-f1c8212b7c03)








   


 


 


 

