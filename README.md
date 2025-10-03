#  Week 1 Shell Navigation Assignment  

This project demonstrates essential **Linux shell commands** for navigation, file management, symbolic links, compression, and system operations. Below are the tasks (1–60) with explanations and example commands.



##  Part 1: Shell Navigation Basics (1–10)

1. **Create a folder named `week1_assignment`:**
   bash
   mkdir week1_assignment
  

2. **Navigate into `week1_assignment`:**
   
   cd week1_assignment
   ```

3. **Create a folder `projects`:**
   ```bash
   mkdir projects
   ```

4. **Create a folder `notes`:**
   ```bash
   mkdir notes
   ```

5. **Create a text file `hello.txt`:**
   ```bash
   touch hello.txt
   ```

6. **Write inside `hello.txt`:**
   ```bash
   echo "Hello WinMingle" > hello.txt
   ```

7. **Inside `projects/`, create `week1_project`:**
   ```bash
   mkdir projects/week1_project
   ```

8. **Inside `week1_project/`, create `main.sh`:**
   ```bash
   touch projects/week1_project/main.sh
   ```

9. **Inside `week1_project/`, create `readme.md`:**
   ```bash
   echo "This is my first project" > projects/week1_project/readme.md
   ```

10. **Go back to `week1_assignment`:**
   ```bash
   cd ..
   ```

---

## 📝 Part 2: Working with Notes (11–20)

11. **Create `day1.txt`:**
   ```bash
   touch notes/day1.txt
   ```

12. **Write into `day1.txt`:**
   ```bash
   echo "Learning shell navigation" > notes/day1.txt
   ```

13. **Create `day2.txt`:**
   ```bash
   touch notes/day2.txt
   ```

14. **Write into `day2.txt`:**
   ```bash
   echo "Second day of practice" > notes/day2.txt
   ```

15. **Create `day3.txt`:**
   ```bash
   echo "Third day assignment" > notes/day3.txt
   ```

16. **Create hidden file `.secret.txt`:**
   ```bash
   echo "hidden knowledge" > notes/.secret.txt
   ```

17. **Append into `day2.txt`:**
   ```bash
   echo "More practice coming" >> notes/day2.txt
   ```

18. **Concatenate into `summary.txt`:**
   ```bash
   cat notes/day1.txt notes/day2.txt > notes/summary.txt
   ```

19. **Count lines in `summary.txt`:**
   ```bash
   wc -l notes/summary.txt > notes/count.txt
   ```

20. **Copy `summary.txt` into backup (later):**
   ```bash
   cp notes/summary.txt backup/
   ```

---

## ⚙️ Part 3: System Operations (21–30)

21. **List contents and save:**
   ```bash
   ls -a > listing.txt
   ```

22. **Create hidden folder `.config`:**
   ```bash
   mkdir .config
   ```

23. **Create `settings.conf`:**
   ```bash
   echo "version=1.0" > .config/settings.conf
   ```

24. **Rename `hello.txt` → `welcome.txt`:**
   ```bash
   mv hello.txt welcome.txt
   ```

25. **Copy `welcome.txt` into `notes/`:**
   ```bash
   cp welcome.txt notes/
   ```

26. **Move `listing.txt` into `projects/`:**
   ```bash
   mv listing.txt projects/
   ```

27. **Create `backup`:**
   ```bash
   mkdir backup
   ```

28. **Copy entire `notes/` into `backup/`:**
   ```bash
   cp -r notes/ backup/
   ```

29. **Print working directory into `pwd.txt`:**
   ```bash
   pwd > pwd.txt
   ```

30. **Append command to `main.sh`:**
   ```bash
   echo "echo Done!" >> projects/week1_project/main.sh
   ```

---

## 🔗 Part 4: Links & Metadata (31–40)

31. **Create symbolic link:**
   ```bash
   ln -s notes/ latest_notes
   ```

32. **Create `userinfo.txt`:**
   ```bash
   echo "Your Full Name" > userinfo.txt
   ```

33. **Append `userinfo.txt` into `day2.txt`:**
   ```bash
   cat userinfo.txt >> notes/day2.txt
   ```

34. **Compress entire folder:**
   ```bash
   zip -r week1_assignment.zip week1_assignment
   ```

35. **Create hidden folder `.gitignore_test`:**
   ```bash
   mkdir projects/week1_project/.gitignore_test
   ```

36. **Inside `.gitignore_test/`, create `ignore.txt`:**
   ```bash
   echo "ignore this" > projects/week1_project/.gitignore_test/ignore.txt
   ```

37. **Copy `userinfo.txt`:**
   ```bash
   cp userinfo.txt projects/userinfo_copy.txt
   ```

38. **Create `logs/`:**
   ```bash
   mkdir logs
   ```

39. **Create `access.log`:**
   ```bash
   echo "log started" > logs/access.log
   ```

40. **Append into `access.log`:**
   ```bash
   echo "log ended" >> logs/access.log
   ```

---

## 📑 Part 5: More Practice (41–50)

41. **Create `draft.txt`:**
   ```bash
   echo "temporary work" > draft.txt
   ```

42. **Move `draft.txt` into `backup/`:**
   ```bash
   mv draft.txt backup/
   ```

43. **Create `numbers.txt` (1–10):**
   ```bash
   seq 1 10 > numbers.txt
   ```

44. **Extract first 5 lines:**
   ```bash
   head -n 5 numbers.txt > first5.txt
   ```

45. **Extract last 5 lines:**
   ```bash
   tail -n 5 numbers.txt > last5.txt
   ```

46. **Merge into `combined.txt`:**
   ```bash
   cat first5.txt last5.txt > combined.txt
   ```

47. **Create `day4.txt`:**
   ```bash
   echo "Fourth day progress" > notes/day4.txt
   ```

48. **Copy `day4.txt` into `projects/`:**
   ```bash
   cp notes/day4.txt projects/
   ```

49. **Create `archive/`:**
   ```bash
   mkdir archive
   ```

50. **Move `combined.txt` into archive:**
   ```bash
   mv combined.txt archive/
   ```

---

## 🕵️ Part 6: Advanced Navigation (51–60)

51. **Create hidden folder `.hidden_data`:**
   ```bash
   mkdir .hidden_data
   ```

52. **Inside it, create `secret.log`:**
   ```bash
   echo "Top Secret" > .hidden_data/secret.log
   ```

53. **Inside `projects/`, create `plan.txt`:**
   ```bash
   echo "future project" > projects/plan.txt
   ```

54. **Append to `plan.txt`:**
   ```bash
   echo "more plans ahead" >> projects/plan.txt
   ```

55. **Create `trash/`:**
   ```bash
   mkdir trash
   ```

56. **Move `draft.txt` (from backup) into `trash/`:**
   ```bash
   mv backup/draft.txt trash/
   ```

57. **Create `timestamp.txt`:**
   ```bash
   date > timestamp.txt
   ```

58. **Create `credits.txt`:**
   ```bash
   echo "Developed by " > credits.txt
   ```

59. **Copy `credits.txt` into `week1_project/`:**
   ```bash
   cp credits.txt projects/week1_project/
   ```

60. **Compress `projects/` into `projects.tar.gz`:**
   ```bash
   tar -czf projects.tar.gz projects/
   ```



## Summary

This assignment covered:
- File & folder creation (`mkdir`, `touch`, `echo`)  
- Navigation (`cd`, `pwd`)  
- File editing & appending (`echo`, `cat`, `>>`)  
- Copying & moving files (`cp`, `mv`)  
- Hidden files & folders (`.` prefix)  
- Symbolic links (`ln -s`)  
- File listing (`ls`)  
- Compression (`zip`, `tar`)  
- Counting lines (`wc`)  

Olayenikan Michael
