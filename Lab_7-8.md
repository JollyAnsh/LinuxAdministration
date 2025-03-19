# **Experiment - 7 & 8**  

*Create the `/home/consultants` directory. Add write permission to the consultants group. Use the symbolic method for setting the appropriate permissions. Forbid others from accessing files in the `/home/consultants` directory. Use the octal method for setting the appropriate permissions. Change the default umask for the operator1 user. The new umask prohibits all access for users that are not in their group. Confirm that the umask is changed.*  
#
### **Approach**  
Use `mkdir` to create a directory. Modify permissions using the symbolic method (`chmod g+w`) and the octal method (`chmod 770`). Update the `umask` setting for `operator1`.  
### **Syntax** 
**`sudo mkdir /home/dir1`**  
Creates a directory named `/home/dir1` with superuser (root) privileges.

**`sudo chmod g+w /home/dir1`**  
Grants write permissions to the group for the `/home/dir1` directory.

**`sudo chmod 770 /home/dir1`**  
Sets the permissions for the `/home/dir1` directory to `rwxrwx---`, allowing the owner and group to read, write, and execute, while others have no permissions.

**`sudo su - user1`**  
Switches to the `user1` user with root privileges, starting a login shell.

**`echo "umask 007" >> ~/.bashrc`**  
Appends `umask 007` to the `~/.bashrc` file, which sets the default permissions for newly created files and directories to `770`.

**`source ~/.bashrc`**  
Reloads the `~/.bashrc` file to apply the changes.

**`umask`**  
Displays the current umask value.

### **Example**
```
sudo mkdir /home/consultants

```
```
sudo chmod g+w /home/consultants

```
```
sudo chmod 770 /home/consultants

```
```
ls -ld /home/consultants

```
```
sudo su - operator1

```
```
echo "umask 007" >> ~/.bashrc

```
```
source ~/.bashrc

```
```
umask

```
Confirm `umask`
```
touch testfile
mkdir testdir
ls -l
```
#
![Screenshot 2025-03-19 194537](https://github.com/user-attachments/assets/d02e76dc-6f82-4aaf-939d-88c5b7c65fe8)
![Screenshot 2025-03-19 194938](https://github.com/user-attachments/assets/9ed45bb7-f6ed-4d81-8301-3cfc378fa587)
![Screenshot 2025-03-19 195035](https://github.com/user-attachments/assets/d708dd51-0602-4ca4-9cc4-7f6babf0e728)


