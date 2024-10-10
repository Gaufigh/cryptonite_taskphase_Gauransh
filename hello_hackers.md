

## Challenge Description: Invoking Intro Command
In this challenge, you are tasked with executing your first command in a Linux shell environment. The goal is to run the `hello` command to retrieve the flag. Linux commands are **case-sensitive**, so typing `hello` correctly is important.

- **Category:** Introductory
- **Objective:** Invoke the `hello` command to retrieve the flag.

---

## Steps to Solve

### 1. **Understanding the Terminal Environment**
Upon starting the challenge, you are greeted with a Linux shell prompt that looks something like this:

```bash
hacker@hello~intro-to-commands:~$
```

This prompt indicates that the system is ready to accept commands from the user.

### 2. **Recognizing Case Sensitivity**
In Linux, commands are **case-sensitive**. This means that `hello`, `Hello`, and `HELLO` are treated as completely different commands. You must enter the command exactly as `hello` in lowercase letters to get the correct result.

### 3. **Executing the Command**
To solve the challenge, you simply need to type the `hello` command at the terminal prompt and hit `Enter`:

```bash
hacker@hello~intro-to-commands:~$ hello
```

### 4. **Retrieving the Flag**
Once you press `Enter`, the shell will execute the command and return the flag. The output will look like this:

```bash
hacker@hello~intro-to-commands:~$ hello
Success! Here is your flag:
pwn.college{wdHoBiJNIgesyEx_ySApYFKl2hh.ddjNyUDL1MzM1czW}
```

The flag is:

```bash
pwn.college{wdHoBiJNIgesyEx_ySApYFKl2hh.ddjNyUDL1MzM1czW}
```



---

## Key Points

- **Case Sensitivity:** Remember that Linux commands are case-sensitive, so you must type the command exactly as instructed.
- **Simple Command Execution:** This challenge introduces basic Linux command execution. You will need to interact with the terminal in this way for future challenges.

---

# Challenge Summary: Invoking `hello` with an Argument

1. **Objective**: Run the `hello` command with the argument `hackers` to retrieve the flag.
   - The command format is: `hello <argument>`

2. **Steps**:
   - Type `hello hackers` and hit enter:
     ```bash
     hacker@hello~intro-to-arguments:~$ hello hackers
     Success! Here is your flag:
     pwn.college{YOISF3n0nDhKXYmtepUq4kEclg_.dhjNyUDL1MzM1czW}
     hacker@hello~intro-to-arguments:~$
     ```

3. **Explanation**: In this command, `hello` is the command you are executing, and `hackers` is the argument passed to it. This command prompts the system to respond with the corresponding flag.




