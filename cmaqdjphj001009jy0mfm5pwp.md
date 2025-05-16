---
title: "🐧 Day 2 - Basic Linux Navigation and File Manipulation for Beginners"
seoTitle: "linux basic commands everything you need to know"
seoDescription: "learn the essential Linux commands every beginner should know! This guide covers basic navigation and file manipulation commands."
datePublished: Fri May 16 2025 05:45:08 GMT+0000 (Coordinated Universal Time)
cuid: cmaqdjphj001009jy0mfm5pwp
slug: day-2-basic-linux-navigation-and-file-manipulation-for-beginners
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1747372544253/0f5e84ce-fb8d-447b-bd62-61425ffc9657.png
tags: linux, navigation, linux-for-beginners, linux-basics, linux-commands, basic-linux-commands

---

Linux is a powerful and widely used operating system, especially in DevOps and server environments. Whether you're managing servers, writing shell scripts, or troubleshooting issues, mastering Linux commands is essential. Here's a guide to the most basic and commonly used Linux commands to get you started.

When you start using Linux, it’s important to first know **who you are**, **where you are**, and then learn how to **move around** and **manage files**.

Before you start creating or managing files, you need to identify yourself and understand your current location in the system

When you're using the **Linux terminal**, the **command prompt** often shows something like this:

## 1\. Username, Hostname, and Working Directory

In the Linux terminal prompt, you often see something like:

```plaintext
username@hostname:working_directory$
```

* **username**: the name of the user currently logged in.
    
* **hostname**: the name of the computer or server.
    
* **working\_directory**: the current folder you are in.
    
* **$**: the prompt symbol indicating a regular user (for root user, it’s `#`).
    
* **Example:**
    
    ```plaintext
    mounika@inspiron:~$
    ```
    
    Here, `mounika` is the user, `inspiron` is the computer name, and `~` means the home directory.
    
    To check these yourself, you can run:
    
    * Your username:
        
        ```plaintext
        whoami
        ```
        
    * Your hostname:
        
        ```plaintext
        hostname
        ```
        
    * Your current directory:
        
        ```plaintext
        pwd
        ```
        
    
    ---
    
    ## 2\. What Does `$` Mean?
    
    * The `$` symbol at the end of the prompt means you are logged in as a **regular user** (non-root).
        
    * If you see `#`, that means you are logged in as the **root user** (administrator).
        
    
    **Example:**
    
    ```plaintext
    mounika@inspiron:~$  (regular user)
    root@inspiron:~#  (root user)
    ```
    

---

## 📂 2. Navigate Through Directories

Linux is like a big tree of folders. You need to learn how to move between these folders.

### 👉 This is Syntax: `ls`

### 👉 This is Structure: Lists files and folders in the current directory.

👉 This is Syntax: `cd foldername`

👉 This is Structure: Changes into the folder called `foldername`.

### 👉 This is Syntax: `cd ..`

👉 This is Structure: Goes back one level to the parent directory.

### 👉 This is Syntax: `cd ~`

👉 This is Structure: Goes to your home directory.

---

## 📄 3. Create and View Files

Now that you know where you are, let’s start making and reading files.

### 📄 How to Create Files in Linux: All Ways Explained with Examples

| Method | Command Example | Description |
| --- | --- | --- |
| `touch` | `touch file.txt` | Create empty file |
| `echo` | `echo "text" > file.txt` | Create file with single line text |
| `cat` | `cat > file.txt` + Ctrl+D | Create file with multiple lines input |
| `printf` | `printf "line1\nline2\n" > file.txt` | Create file with formatted content |
| Text Editors | `nano file.txt` or `vim file.txt` | Create and edit file interactively |

### 1\. Using `touch` command

* **Purpose:** Creates an empty file or updates the timestamp of an existing file.
    
* **Syntax:**
    
    ```plaintext
    touch filename.txt
    ```
    
* **Example:**
    
    ```plaintext
    touch myfile.txt
    ```
    
    Creates an empty file called `myfile.txt` if it doesn't exist.
    

### 👉 This is Syntax: `touch filename.txt`

### 2\. Using `echo` command

* **Purpose:** Create a file and add some text content to it.
    
* **Syntax:**
    
    ```plaintext
    echo "Your text here" > filename.txt
    ```
    
* **Example:**
    
    ```plaintext
    echo "Hello Linux!" > greetings.txt
    ```
    
    Creates `greetings.txt` with the content `Hello Linux!`.
    
* **Note:**  
    Using `>` will overwrite the file if it exists. Use `>>` to append text.
    

---

### 3\. Using `cat` command

* **Purpose:** Create a file and enter multiple lines manually.
    
* **Syntax:**
    
    ```plaintext
    cat > filename.txt
    ```
    
    Then type text, and press `Ctrl + D` to save and exit.
    
* **Example:**
    
    ```plaintext
    cat > notes.txt
    ```
    
    Then type:
    
    ```plaintext
    This is my first note.
    This is the second line.
    ```
    
    Press `Ctrl + D` when done.
    

---

### 4\. Using `printf` command

* **Purpose:** Create a file with formatted content.
    
* **Syntax:**
    
    ```plaintext
    printf "Line1\nLine2\n" > filename.txt
    ```
    
* **Example:**
    
    ```plaintext
    printf "Hello\nWorld\n" > hello.txt
    ```
    
    Creates `hello.txt` with two lines:
    
    ```plaintext
    Hello
    World
    ```
    

---

### 5\. Using text editors

* **Purpose:** Create and edit files interactively.
    
* **Common editors:**
    
    * `nano filename.txt` — Easy-to-use text editor.
        
    * `vim filename.txt` — Powerful but advanced editor.
        
* **Example with nano:**
    
    ```plaintext
    nano myfile.txt
    ```
    
    This opens the nano editor where you can write content, then save (`Ctrl + O`) and exit (`Ctrl + X`).
    

---

* ## **👀 Viewing Files in Linux: Commands and Examples**
    
* ### 1\. `cat` — View entire file content
    
    * **Syntax:**
        
        ```plaintext
        cat filename.txt
        ```
        
    * **Example:**
        
        ```plaintext
        cat myfile.txt
        ```
        
        Displays the full content of `myfile.txt` on the terminal.
        
    * **Note:** Good for small files because it prints all content at once.
        
    
    ---
    
    ### 2\. `head` — View the first few lines of a file
    
    * **Syntax:**
        
        ```plaintext
        head filename.txt
        ```
        
        By default, shows the first 10 lines.
        
    * **Example:**
        
        ```plaintext
        head myfile.txt
        ```
        
        Shows the first 10 lines of `myfile.txt`.
        
    * **View specific number of lines:**
        
        ```plaintext
        head -n 5 myfile.txt
        ```
        
        Shows first 5 lines.
        
    
    ---
    
    ### 3\. `tail` — View the last few lines of a file
    
    * **Syntax:**
        
        ```plaintext
        tail filename.txt
        ```
        
        Shows last 10 lines by default.
        
    * **Example:**
        
        ```plaintext
        tail myfile.txt
        ```
        
        Displays last 10 lines.
        
    * **View specific number of lines:**
        
        ```plaintext
        tail -n 7 myfile.txt
        ```
        
        Shows last 7 lines.
        
    * **Follow file changes live:**
        
        ```plaintext
        tail -f /var/log/syslog
        ```
        
        Keeps showing new lines added to the file in real time (useful for logs).
        
    
    ---
    
    ### 4\. `less` — View file page by page (scrollable)
    
    * **Syntax:**
        
        ```plaintext
        less filename.txt
        ```
        
    * **Example:**
        
        ```plaintext
        less myfile.txt
        ```
        
        Opens the file for easy navigation up/down.
        
    * **Navigation keys:**
        
        * Press `Space` to go to next page
            
        * Press `b` to go back one page
            
        * Use arrow keys to scroll line by line
            
        * Press `q` to quit
            
    
    ---
    
    ### 5\. `more` — View file page by page (basic)
    
    * **Syntax:**
        
        ```plaintext
        more filename.txt
        ```
        
    * **Example:**
        
        ```plaintext
        more myfile.txt
        ```
        
        Similar to `less` but with fewer features.
        
    
    ---
    
    ### Summary Table
    
    | Command | Purpose | Example |
    | --- | --- | --- |
    | `cat` | View full file content | `cat file.txt` |
    | `head` | View first 10 lines | `head file.txt` |
    | `head -n N` | View first N lines | `head -n 5 file.txt` |
    | `tail` | View last 10 lines | `tail file.txt` |
    | `tail -n N` | View last N lines | `tail -n 7 file.txt` |
    | `tail -f` | Follow live file updates | `tail -f /var/log/syslog` |
    | `less` | Scrollable view, page-wise | `less file.txt` |
    | `more` | Basic scrollable view | `more file.txt` |
    

---

* ## 📁 Managing Directories in Linux: Commands and Examples
    
    ---
    
    ## What is a Directory?
    
    * A **directory** is like a folder that holds files and other directories.
        
    * Directories help organize your files on Linux systems.
        
    
    ---
    
    ## Common Directory Management Commands
    
    ### 1\. **Create a Directory:** `mkdir`
    
    * **Syntax:**
        
        ```plaintext
        mkdir directory_name
        ```
        
    * **Example:**
        
        ```plaintext
        mkdir projects
        ```
        
        Creates a new directory named `projects`.
        
    * **Create multiple directories at once:**
        
        ```plaintext
        mkdir dir1 dir2 dir3
        ```
        
    * **Create parent directories as needed:**
        
        ```plaintext
        mkdir -p parent/child/grandchild
        ```
        
        Creates the full nested directory structure even if the parents don’t exist.
        
    
    ---
    
    ### 2\. **Change Directory:** `cd`
    
    * **Syntax:**
        
        ```plaintext
        cd directory_path
        ```
        
    * **Example:**
        
        ```plaintext
        cd projects
        ```
        
        Moves into the `projects` directory.
        
    * **Other useful shortcuts:**
        
        * `cd ..` → Move up one directory (to parent directory)
            
        * `cd ~` or simply `cd` → Go to your home directory
            
        * `cd -` → Switch back to the previous directory
            
    
    ---
    
    ### 3\. **List Directory Contents:** `ls`
    
    * **Syntax:**
        
        ```plaintext
        ls [options] [directory]
        ```
        
    * **Example:**
        
        ```plaintext
        ls
        ```
        
        Lists files and folders in the current directory.
        
    * **Common options:**
        
        * `ls -l` → Detailed list with permissions, size, and modification date
            
        * `ls -a` → Show all files including hidden ones (those starting with `.`)
            
        * `ls -lh` → Human-readable sizes (KB, MB)
            
    
    ---
    
    ### 4\. **Remove a Directory:** `rmdir` and `rm`
    
    * **Remove empty directory:**
        
        ```plaintext
        rmdir directory_name
        ```
        
    * **Remove directory with files inside:**
        
        ```plaintext
        rm -r directory_name
        ```
        
        Use `-r` (recursive) to delete directory and its contents.
        
    * **Force remove without prompt:**
        
        ```plaintext
        rm -rf directory_name
        ```
        
        Be very careful! This deletes directory and everything inside without confirmation.
        
    
    ---
    
    ### 5\. **Print Current Directory:** `pwd`
    
    * **Syntax:**
        
        ```plaintext
        pwd
        ```
        
    * **Example:**
        
        ```plaintext
        pwd
        ```
        
        Shows the full path of your current working directory.
        
    
    ---
    
    ## Summary Table
    
    | Command | Description | Example |
    | --- | --- | --- |
    | `mkdir directory` | Create new directory | `mkdir myfolder` |
    | `mkdir -p parent/child` | Create nested directories | `mkdir -p projects/app/src` |
    | `cd directory` | Change directory | `cd projects` |
    | `cd ..` | Go to parent directory | `cd ..` |
    | `ls` | List files and folders | `ls -la` |
    | `rmdir directory` | Remove empty directory | `rmdir oldfolder` |
    | `rm -r directory` | Remove directory with contents | `rm -r oldfolder` |
    | `pwd` | Print current directory path | `pwd` |
    

---

* ## ✂️ 5. Copy, Move, and Delete Files
    
    ---
    
    ## Copy Files (`cp`)
    
    * **Syntax:**
        
        ```plaintext
        cp source_file destination_file
        ```
        
    * **Example:**
        
        ```plaintext
        cp file1.txt file2.txt
        ```
        
        Copies `file1.txt` to `file2.txt`.
        
    * **Copy directories recursively:**
        
        ```plaintext
        cp -r folder1 folder2
        ```
        
        Copies `folder1` and its contents to `folder2`.
        
    
    ---
    
    ## Move or Rename Files (`mv`)
    
    * **Syntax:**
        
        ```plaintext
        mv old_name new_name
        ```
        
    * **Example (rename):**
        
        ```plaintext
        mv oldname.txt newname.txt
        ```
        
    * **Example (move to directory):**
        
        ```plaintext
        mv filename.txt /path/to/destination/
        ```
        
    
    ---
    
    ## Delete Files (`rm`)
    
    * **Syntax:**
        
        ```plaintext
        rm filename
        ```
        
    * **Example:**
        
        ```plaintext
        rm file.txt
        ```
        
    * **Delete directories recursively:**
        
        ```plaintext
        rm -r myfolder
        ```
        
    * **Force delete without prompt:**
        
        ```plaintext
        rm -rf myfolder
        ```
        
    
* ## ✅ Conclusion
    
    These basic commands are the building blocks of using Linux. Once you’re confident with them, you’ll be able to:
    
    * Explore directories 🚶‍♀️
        
    * Create files and folders 📁
        
    * Organize your data 🗂️
        
    * Understand your system better 💻
        
    
    Practice them regularly, and Linux will become your best friend!