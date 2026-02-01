Here are **30 practical, progressive file handling challenges** in Python. They start from absolute basics and gradually become more realistic/useful (especially for scripting, automation, and later red team / security contexts).

Do them **in order** — each builds on previous concepts. Use `with open(...)` everywhere, handle basic exceptions (like `FileNotFoundError`), and test with real small files you create.

### Level 1 – Very Basic (1–8)

1. Create an empty file called `test.txt` (use `'w'` mode).

solue:
```bash
try:
    with open("null.txt","w") as f:
        pass

except Exception as e:
    print(f"error:{e}")
    
````
2. Write your full name into `info.txt` as a single line.

3. Append the current date/time (use `datetime.now()`) to `log.txt` (append mode).

4. Read and print the entire content of `info.txt`.

5. Read `log.txt` line by line and print each line with line numbers (1. ..., 2. ...).

6. Count and print how many lines are in any text file (e.g., copy-paste a paragraph into `story.txt`).

7. Read a file and print only lines that contain the word "python" (case insensitive).

8. Create a file `numbers.txt` and write numbers 1 to 50, each on its own line.

### Level 2 – Reading & Simple Processing (9–15)

9. Read `numbers.txt` (from #8) and calculate the sum of all numbers.

10. Read a text file and count total words (split on spaces).

11. Read a file and return a dictionary: {"lines": count, "words": count, "chars": count} (without spaces or with spaces — your choice).

12. Read a CSV-like file (e.g., create `students.csv` with "name,age,city" lines) and print each student as "Name: ..., Age: ..., City: ...".

13. Read any file and reverse every line (characters reversed), write to `reversed.txt`.

14. Read a file, remove all empty lines (or lines with only whitespace), write cleaned version to new file.

15. Read two files (`file1.txt` and `file2.txt`), merge them line-by-line into `merged.txt`.

### Level 3 – Writing & Transformation (16–22)

16. Ask user for 5 lines of input → write them to `user_notes.txt`.

17. Copy the content of one file to another (simple copy — read whole → write whole).

18. Copy a file but add line numbers at the beginning of each line (like code listing).

19. Read a file, replace every occurrence of "old" with "new", write to new file.

20. Read a log file, extract only lines containing "ERROR" or "WARNING", write them to `errors.txt`.

21. Create a file `multiplied.txt` where each number from `numbers.txt` is multiplied by 10.

22. Read a text file, count frequency of each word (use dict), write top 5 most common words to `wordcount.txt`.

### Level 4 – os / shutil / pathlib + Real-world-ish (23–27)

23. Check if a file exists before reading it (print message if not found).

24. Rename a file using `os.rename()` (e.g., `old.txt` → `new_name.txt`).

25. Delete a file if it exists (`os.remove()`), but ask user for confirmation first.

26. Copy an entire folder recursively using `shutil.copytree()` (create small test folder with 2–3 files).

27. Use `pathlib`: List all `.txt` files in current directory (and subfolders with `rglob`).

### Level 5 – Binary + a bit harder / useful patterns (28–30)

28. Copy a binary file (e.g., small image `photo.jpg` → `backup.jpg`) using binary mode `'rb'` / `'wb'`.

29. Read a binary file in chunks of 1024 bytes and print total size in KB/MB.

30. (Mini project) Write a simple "file splitter": read large text file, split every 100 lines into new files (`part1.txt`, `part2.txt`, ...).

### How to Approach These

- Create a folder like `file_practice/`  
- Put all your test files there  
- Make one `.py` file per challenge (or one big file with functions)  
- After each 5–7 tasks, try combining them (e.g., clean file → count words → save stats)  
- Use meaningful variable names and comments  
- Always close files with `with` — never forget!

When you finish ~20 of these, file handling will feel natural and you'll be ready for `requests`, `os`/`shutil` heavy scripting, parsing logs, credential dumping simulation, etc.

If you want **sample starter code** or **expected output** for any specific task (or solutions after you try), just tell me the number!

Which one do you want to start with right now? Or shall we jump to `requests` after you do the first 10?
