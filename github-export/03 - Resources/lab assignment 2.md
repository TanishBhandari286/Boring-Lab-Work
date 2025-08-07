# LAB ASSIGNMENT NO. 2

**Aim:** To learn and implement file handling

---

## q1  
**a1**  
**Question:** Create files `myfile_NAME` and `yourfile_NAME` under the Present Working Directory.  
**command used:**  
```bash
touch myfile_NAME yourfile_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.17.20@2x.png)
---

## q2  
**a2**  
**Question:** Display the files `myfile_NAME` and `yourfile_NAME`.  
**command used:**  
```bash
cat myfile_NAME yourfile_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.18.11@2x.png)

---

## q3  
**a3**  
**Question:** Append more lines in the `myfile_NAME` and `yourfile_NAME` files.  
**command used:**  
```bash
echo >> This is line 1 >> myfile_NAME
echo >> This is lline 2 >> yourfile_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.19.52@2x.png)

---

## q4  
**a4**  
**Question:** How will you create a hidden file?  
**command used:**  
```bash
nvim .bashrc
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.20.31@2x.png)
---

## q5  
**a5**  
**Question:** Copy `myfile_NAME` file to `emp_NAME`.  
**command used:**  
```bash 
echo > myfile_NAME emp_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.22.13@2x.png)
---

## q6  
**a6**  
**Question:** Move `yourfile_NAME` file to `dept_NAME`.  
**command used:**  
```bash 
cp yourfile_NAME ~/os/dept_name
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.28.10@2x.png)
---

## q7  
**a7**  
**Question:** Copy `emp_NAME` file and `dept_NAME` file to `TRIAL_NAME` directory.  
**command used:**  
```bash
cat emp_NAME dep_name > TRIAL_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.30.43@2x.png)
---

## q8  
**a8**  
**Question:** Compare a file with itself.  
**command used:**  
```bash
diff yourfile_NAME yourfile_NAME 
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.31.49@2x.png)
---

## q9  
**a9**  
**Question:** Compare `myfile_NAME` file and `emp_NAME` file.  
**command used:**  
```bash
 diff myfile_NAME emp_NAME 
 ```
**output:**  
![](CleanShot%202025-08-05%20at%2011.32.51@2x.png)
---

## q10  
**a10**  
**Question:** Append two more lines in `emp_NAME` file existing in `TRIAL_NAME` directory.  
**command used:**  
```bash
echo "First new line" >> ./tanish.txt
echo "Second new line" >> ./tanish.txt
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.42.49@2x.png)
---

## q11  
**a11**  
**Question:** Compare `employee_NAME` file with `emp_NAME` file in `TRIAL_NAME` directory.  
**command used:**  
```bash
diff employeename empname
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.44.26@2x.png)
---

## q12  
**a12**  
**Question:** Find the difference between the above two files.  
**command used:**  
```bash
diff -u employeename empname
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.45.32@2x.png)
---

## q13  
**a13**  
**Question:** Remove the files in the `TRIAL_NAME` directory.  
**command used:**  
```bash 
rm -rf *
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.46.20@2x.png)
---

## q14  
**a14**  
**Question:** Can you remove a directory with files by using a single command?  
**command used:**  
```bash
rm -rf <dir_name>
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.47.00@2x.png)
---

## q15  
**a15**  
**Question:** Is there any command available to get back a deleted file?  
**command used:**  
```bash
no command to retrieve it 
```
**output:**  

---

## q16  
**a16**  
**Question:** Rename `TRIAL_NAME` as `DATA_NAME`.  
**command used:**  
```bash
mv TRIAL_NAME DATA_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.47.52@2x.png)

---

## q17  
**a17**  
**Question:** Copy `DATA_NAME` to another directory by name `TRIAL_NAME`.  
**command used:**  
```bash
cp DATA_NAME ./TRIAL_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.49.02@2x.png)
---

## q18  
**a18**  
**Question:** Write the command to create an alias name for a file.  
**command used:**
```
v ~/.bashrc

added alias
alias editbrew = nvim ~/.brewfile
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.56.43@2x.png)
---

## q19  
**a19**  
**Question:** Create a file called `dummy_NAME` in `TRIAL_NAME` and link it to another file by name `star_NAME`.  
**command used:**  
```bash
ln star_NAME dummy_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.53.02@2x.png)
---

## q20  
**a20**  
**Question:** Link the `dummy_NAME` file in `TRIAL_NAME` to another file by name `power_NAME` in `DATA_NAME`.  

**command used:**  
```bash
ln -s ../DATA_NAME/power_NAME dummy_NAME
```
**output:**  
![](CleanShot%202025-08-05%20at%2011.55.19@2x.png)
---
