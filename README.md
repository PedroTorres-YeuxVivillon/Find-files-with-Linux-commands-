# 🐧 Linux Basics: Navigating Directories and Finding Files

This repository documents my hands-on lab with essential Linux Bash shell commands. As a beginner in cybersecurity and system administration, knowing how to efficiently navigate and inspect files from the command line is a critical skill.

## 📖 Project Overview

This lab simulated a common task for an analyst: exploring a filesystem without a graphical interface to locate and analyze specific files. My goal was to navigate through directories, list their contents, and read files to extract important information.

The scenario involved investigating user reports and server logs located within the `/home/analyst` directory.

### **What I Learned & Practiced**

*   **`pwd`** (Print Working Directory): To confirm my current location in the filesystem.
*   **`ls`** (List): To view the contents of a directory.
*   **`cd`** (Change Directory): To navigate between different folders.
*   **`cat`** (Concatenate): To display the entire contents of a file.
*   **`head`**: To display only the first few lines of a file.

## 🛠️ Lab Tasks & My Solutions

### **Task 1: Explore the Starting Directory**

**Goal:** Identify my current working directory and see what it contains.

**My Commands & Steps:**
1.  I used `pwd` to print the absolute path of my current directory.
    ```bash
    pwd
    ```
2.  I used `ls` to list all the files and subdirectories in this location.
    ```bash
    ls
    ```

**Findings:**
*   **Current Directory:** `/home/analyst`
*   **Number of Subdirectories:** The output showed several items. After counting the directories (which are often highlighted in blue), I found there were **Four** subdirectories.

---

### **Task 2: Navigate to the Reports Directory**

**Goal:** Change into the `reports` directory and identify its subfolders.

**My Commands & Steps:**
1.  I used `cd` to move into the `reports` directory.
    ```bash
    cd /home/analyst/reports
    ```
2.  I ran `ls` again to see what was inside.
    ```bash
    ls
    ```

**Findings:**
*   **Subdirectory Name:** The `reports` directory contained one subdirectory named **`users`**.

---

### **Task 3: Find and Read a User Report**

**Goal:** Navigate to the `users` directory and examine the contents of a specific file to answer questions about employees.

**My Commands & Steps:**
1.  I changed into the `users` directory.
    ```bash
    cd users
    ```
2.  I listed the files to find `Q1_added_users.txt`.
    ```bash
    ls
    ```
3.  I used `cat` to display the entire contents of the file.
    ```bash
    cat Q1_added_users.txt
    ```

**Findings:**
After reading the file, which contained a list of usernames, employee IDs, and departments, I found:
*   The user `aezra` works in the **Human Resources** department.
*   The user `mreed` in the **Information Technology** department has the employee ID **1188**.

---

### **Task 4: Analyze Server Logs**

**Goal:** Navigate to the `logs` directory and examine the beginning of a server log file to count warning messages.

**My Commands & Steps:**
1.  I navigated directly to the `/home/analyst/logs` directory.
    ```bash
    cd /home/analyst/logs
    ```
2.  I listed the contents to find the log file.
    ```bash
    ls
    ```
3.  I used the `head` command to output only the first 10 lines of the `server_logs.txt` file.
    ```bash
    head server_logs.txt
    ```

**Findings:**
By carefully reading the first 10 lines of the log, I counted each line that contained the word "WARNING".
*   **Number of Warnings:** There were **Three** warning messages in the first 10 lines.

## ✅ Conclusion

This lab provided practical, hands-on experience with core Linux commands. I successfully learned how to:

*   Orient myself within a filesystem using `pwd`.
*   Move seamlessly between directories using `cd`.
*   Inspect directory contents using `ls`.
*   Read entire files with `cat` and partial files with `head` to efficiently find information.

These skills form the foundation for all advanced command-line work, from system administration and security analysis to software development.

