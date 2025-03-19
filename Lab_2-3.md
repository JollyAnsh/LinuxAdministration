# **Experiment - 2 & 3**  

*View the gedit man page. Use the `man -k ext4` command to find the command to tune ext4 file-system parameters. Brace expansion is used to generate discretionary strings of characters. Braces contain a comma-separated list of strings, or a sequence expression. The result includes the text that precedes or follows the brace definition.*  
#
### **Approach**  
Use the `man` command to view manual pages and search for commands related to `ext4`. Utilize brace expansion to generate sequences efficiently.  
### **Syntax**  

**`man [command]`**  
   Displays the manual page for the specified command.  

**`man -k [keyword]`**  
   Searches for the keyword in the manual pages and lists all matching entries.  

**`echo [pattern]`**  
   Outputs the result of a pattern or variable expansion.  

**`echo {start..end}`**  
   Expands a range of values from `start` to `end` and outputs the result.  

### **Example**
```
man gedit

```

```
man -k ext4

```

```
echo file{1,2,3}.txt

```

```
echo {a..e}

```
#
![Screenshot 2025-03-19 182713](https://github.com/user-attachments/assets/99da0ea4-88ac-4ccd-b346-6bf5337cd976)
![Screenshot 2025-03-19 182751](https://github.com/user-attachments/assets/b1690b1c-eb33-4302-8dc1-5c09a9407980)
#
![Screenshot 2025-03-19 183147](https://github.com/user-attachments/assets/b6fd6b97-e99a-49bf-8cf4-23f0079ce303)
#
![Screenshot 2025-03-19 183307](https://github.com/user-attachments/assets/47fbcf63-3704-46d1-b0cf-f924343c9163)
