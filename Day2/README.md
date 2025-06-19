# 🐧 Day 02: Kali Linux Basics – Cybersecurity Training

## 📁 Section 1: Basic Kali Linux Commands

> A summary of commonly used terminal commands for navigation and file management in Kali Linux.

### 🔍 System Information

```bash
uname -a         # Displays kernel version and system architecture
hostname         # Shows the system's hostname
whoami           # Displays the currently logged in user
```

### 📈 Understanding Users and Privileges

> Kali Linux uses a privilege model to control user access.

* `whoami` shows the current logged-in username.
* `sudo su` switches to root user (if permitted).
* `sudo -l` lists allowed (and forbidden) sudo commands for the user.
* `sudo su -l` switches to a login shell as root.

### 📷 Add Screenshot Here

```
![image](https://github.com/user-attachments/assets/b4ccbefa-f705-40f0-ad2c-5fbcc653c714)
![image](https://github.com/user-attachments/assets/718c1f33-f939-434e-9b1f-5d216966491d)
![image](https://github.com/user-attachments/assets/8019551a-a13f-446b-b4df-56eb7128cbd4)
![image](https://github.com/user-attachments/assets/17b89a76-5d21-42b5-82d4-ba1c8e164ffa)
```

---
## 👤 Section: Adding a User in Kali Linux

> In Kali Linux, managing users and their privileges is essential for secure multi-user operations. Here's how to add a user step-by-step.

---
### ➕ Step 1: Add a New User
```bash
sudo adduser newusername
```
1.This command creates a new user.
2.You will be prompted to set the password and optionally fill in other user info.


###🛡️ Step 2: Grant Sudo Privileges (Optional)
```bash
sudo usermod -aG sudo newusername
```
1.Adds the user to the sudo group.
2.Gives administrative/root-level permission.

```bash
su - newusername
```
###📄 Step 4: Verify if the User Exists
```bash
cat /etc/passwd | grep newusername

```
.Confirms the user is created by checking /etc/passwd
### 📂 Navigation

```bash
pwd              # Shows current working directory
ls               # Lists files in a directory
ls -la           # Lists all files including hidden ones with details
cd /path/to/dir  # Changes directory
```

### 📄 File & Directory Operations

```bash
mkdir dirname    # Creates a new directory
rmdir dirname    # Deletes an empty directory
rm filename      # Deletes a file
rm -r dirname    # Deletes a directory and its contents
touch filename   # Creates a new empty file
cat filename     # Displays content of a file
```

### 📷 Add Screenshot Here

```
![image](https://github.com/user-attachments/assets/768f00d1-567f-405c-9494-05225b73d8a4)
![image]![image](https://github.com/user-attachments/assets/991e9c54-430c-4c7b-814f-0335e888db4d)


```

---

## 👤 Section 2: Adding a User in Kali Linux

> Steps to create a new user with and without admin privileges

### ➕ Add a New User

```bash
sudo adduser newusername
```

* You’ll be prompted to set the password and enter optional user info (can be skipped).

### 🛡️ Add User to Sudo Group (Optional)

```bash
sudo usermod -aG sudo newusername
```

* This grants administrative privileges to the new user.

### 🔐 Switch User

```bash
su - newusername
```

### 📟 Confirm User Exists

```bash
cat /etc/passwd | grep newusername
```

### 📷 Add Screenshot Here

```
![Add User Screenshot](path-to-screenshot.png)
```

---

## 📌 Notes

* Always use `sudo` when performing administrative tasks.
* Avoid using root directly unless necessary.

---

## 🔗 References

* [Kali Linux Documentation](https://www.kali.org/docs/)
* \[Linux Command Cheat Sheet]\([https://lin](https://lin)
