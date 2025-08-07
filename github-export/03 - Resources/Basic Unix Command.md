# **LAB ASSIGNMENT NO. 1**

## **Aim: Basic UNIX Commands**

---

### **Q1. Obtain the following results**

#### i. To Print the name of Operating System:

**Command used:**
```bash
		uname
```
**Explanation:**

The `uname` command displays the operating system of the machine.

**Output:**
![](CleanShot%202025-08-04%20at%2013.26.38@2x.png)

---

#### ii. To Print the login name:

**Command used:**
```bash
logname
```

**Explanation:**

Logname command gives you the name of the user logged into the system 

**Output:**

![](CleanShot%202025-08-04%20at%2013.27.53@2x.png)
---

#### iii. To Print the host name:

**Command used:**
```bash
hostname
```

**Explanation:**

Hostname command gives you the hostname of your machine which u would have setup while entering machine name at the time of installing OS


**Output:**
![](CleanShot%202025-08-04%20at%2013.29.21@2x.png)


---

### **Q2. Find out the users who are currently logged in and find the particular user too.**

**Command used:**

```bash
who
```

**Explanation:**
who command gives you the info about the logged in users and also the mode from which they are logged in


**Output:**
![](CleanShot%202025-08-04%20at%2013.30.55@2x.png)


---

### **Q3. Display the calendar for**

#### i. Jan 2000

#### ii. Feb 1999

#### iii. 7th, 8th, and 9th month of the year 2000

#### iv. For the Current Month

#### v. Current Date, Day Abbreviation, Month Abbreviation, and Year

**Command used:**

```bash
cal 1 2000
cal 2 1999
cal 7 2000; cal 8 2000; cal 9 2000
cal
date "+%d %a %b %Y"
```


**Explanation:**
cal command is a versatile command that can have many flags and to get the desired output we need to use the correct format / flags that cal supports

like - cal 1 2000 Displays the **calendar for January 2000**.
    
- `1` is the month and `2000` is the year.

cal 2 1999
Displays the calendar for February 1999.

cal 7 2000;
cal 8 2000;
cal 9 2000
Displays the calendar for July, August, and September 2000.
cal
Displays the calendar for the current month and year based on the system date.

date "+%d %a %b %Y"
Displays the current date in the format:

%d = Day 

%a = Abbreviated day of the week 

%b = Abbreviated month name 

%Y = Full year 

**Output:**

![](CleanShot%202025-08-04%20at%2013.35.13@2x.png)

![](CleanShot%202025-08-04%20at%2013.35.58@2x.png)

![](CleanShot%202025-08-04%20at%2013.36.32@2x.png)

---

### **Q4. Display the time in 12-Hour and 24-Hour Notations.**

**Command used:**
```bash
date +"%r"
date +"%T"
```


**Explanation:**
- `date +"%r"` displays the current time in **12-hour format with AM/PM**.
    
- `date +"%T"` displays the current time in **24-hour format (HH:MM:SS)**



**Output:**
![](CleanShot%202025-08-04%20at%2013.37.45@2x.png)


---

### **Q5. Display the Current Date and Current Time.**

**Command used:**

```bash
date
```

**Explanation:**
The `date` command displays the **current system date and time** in the default format (e.g., `Mon Aug 4 13:38:00 IST 2025`).


**Output:**

![](CleanShot%202025-08-04%20at%2013.38.42@2x.png)

---

### **Q6. Display the message “GOOD MORNING” in enlarged characters.**

**Command used:**
```bash
banner "GOOD MORNING"
```

**Explanation:**

Banner command in unix is used to display a text in enlarged format using ascii just like toilet command


**Output:**
![](CleanShot%202025-08-04%20at%2013.40.10@2x.png)


---

### **Q7. Display the name of your home directory.**

**Command used:**
```bash
echo $HOME
```

**Explanation:**

Echo just prints the output , $ sign computes it as an expression and home is the directory about which we want to do


**Output:**

![](CleanShot%202025-08-04%20at%2013.41.32@2x.png)

---

### **Q8. Create a directory `SAMPLE_NAME` under your home directory.**

**Command used:**
```bash
mkdir SAMPLE_NAME
```

**Explanation:**
mkdir creates a directory named `SAMPLE_NAME under the path it was called in our case ~


**Output:**

![](CleanShot%202025-08-04%20at%2013.42.37@2x.png)

---

### **Q9. Create a Sub-directory by name `TRIAL_NAME` under `SAMPLE_NAME`.**

**Command used:**

```bash
cd SAMPLE_NAME
mkdir TRIAL_NAME
```

**Explanation:**

as mkdir creates a directory in the active path so first we cd into the sample name and then create it


**Output:**
![](CleanShot%202025-08-04%20at%2013.43.11@2x.png)


---

### **Q10. Change to `SAMPLE_NAME`.**

**Command used:**
```bash
cd SAMPLE_NAME
```


**Explanation:**

cd changes the active directory and places us in the desired directory

**Output:**

![](CleanShot%202025-08-04%20at%2013.45.59@2x.png)

---

### **Q11. Change to your home directory.**

**Command used:**
```bash
cd
```


**Explanation:**
if cd left empty or without flag it places u to the last directory your user has access to


**Output:**
![](CleanShot%202025-08-04%20at%2013.46.49@2x.png)


---

### **Q12. Change from home directory to `TRIAL_NAME` by using absolute and relative pathname.**

**Command used:**
```bash
 cd /Users/tanish/SAMPLE_NAME/TRIAL_NAME
 cd ~/SAMPLE_NAME/TRIAL_NAME
```


**Explanation:**

u can cd using both relative path and absolute path although for simplicity we always use ~ while cd’ing into something

**Output:**

![](CleanShot%202025-08-04%20at%2013.47.40@2x.png)

---

### **Q13. Remove directory `TRIAL_NAME`.**

**Command used:**
```bash
rm -rf TRIAL_NAME
```


**Explanation:**
rm means remove and -rf flag means forcefully and recursively


**Output:**

![](CleanShot%202025-08-04%20at%2013.49.12@2x.png)

---

### **Q14. Create a directory `TEST_NAME` under `SAMPLE_NAME` using absolute pathname.**

**Command used:**

```bash
mkdir TEST_NAME
```

**Explanation:**

as mkdir creates a directory in the active path so first we cd into the sample name and then create it

**Output:**

![](CleanShot%202025-08-04%20at%2013.50.49@2x.png)

---

### **Q15. Using a single command change from current directory to previous directory.**

**Command used:**
```bash
cd ..
```


**Explanation:**
cd .. takes u to the just previous directory relative to your active directory


**Output:**

![](CleanShot%202025-08-04%20at%2013.51.40@2x.png)

---

### **Q16. Remove directory `TEST_NAME` using absolute pathname.**

**Command used:**
```bash
 rm -rf /Users/tanish/SAMPLE_NAME/TEST_NAME
```


**Explanation:**
rm means remove and -rf flag means forcefully and recursively


**Output:**
![](CleanShot%202025-08-04%20at%2013.52.20@2x.png)
