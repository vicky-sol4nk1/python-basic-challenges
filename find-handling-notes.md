Here are the **updated notes** from the same video (Lecture 7: File Input/Output in Python), now with **short, clear examples** added for every major point — exactly as you asked.

### 1. Opening a File
```python
f = open("data.txt", "r")     # read mode (default)
f = open("log.txt", "w")      # write (creates or overwrites)
f = open("notes.txt", "a")    # append (adds at end)
f = open("image.png", "rb")   # binary read
```

### 2. Best Practice: `with` statement (auto close + safe)
```python
with open("story.txt", "r") as file:
    content = file.read()
    print(content)            # file closes automatically even if error occurs
```

### 3. Reading Methods

- `read()` → whole file as string
```python
with open("names.txt") as f:
    all_text = f.read()
    print(all_text)
```

- `readline()` → one line at a time
```python
with open("log.txt") as f:
    first_line = f.readline()      # "2025-02-01 ERROR\n"
    second_line = f.readline()
```

- `readlines()` → list of all lines
```python
with open("config.txt") as f:
    lines = f.readlines()
    print(lines[0])                # first line
```

- Loop directly (best for large files)
```python
with open("access.log") as f:
    for line in f:
        if "ERROR" in line:
            print(line.strip())
```

### 4. Writing Methods

- `write()` (no automatic newline)
```python
with open("output.txt", "w") as f:
    f.write("Hello")
    f.write("World\n")           # manual \n
```

- `writelines()` (list of strings)
```python
lines = ["Line 1\n", "Line 2\n", "Line 3\n"]
with open("newfile.txt", "w") as f:
    f.writelines(lines)
```

- Append example
```python
with open("log.txt", "a") as f:
    f.write("New entry at 14:30\n")
```

### 5. File Positions & Seeking

```python
with open("data.txt", "r") as f:
    print(f.tell())           # 0 (start)
    f.read(10)                # read first 10 bytes
    print(f.tell())           # 10
    
    f.seek(0)                 # back to beginning
    print(f.read(5))          # first 5 chars again
    
    f.seek(0, 2)              # go to end
    print(f.tell())           # file size in bytes
```

### 6. Common Real Patterns

- Copy file content
```python
with open("source.txt", "r") as src, open("copy.txt", "w") as dest:
    dest.write(src.read())
```

- Count lines
```python
count = 0
with open("bigfile.txt") as f:
    for _ in f:
        count += 1
print("Lines:", count)
```

- Simple CSV-like split
```python
with open("users.csv") as f:
    for line in f:
        fields = line.strip().split(",")
        print("Name:", fields[0], "Age:", fields[1])
```

### 7. Binary Files (images, executables, etc.)

```python
# Copy an image
with open("photo.jpg", "rb") as src, open("backup.jpg", "wb") as dest:
    dest.write(src.read())
```

### 8. Other Useful Functions

```python
import os
import shutil

os.remove("temp.txt")                  # delete file
os.rename("old.txt", "new_name.txt")   # rename

print(os.path.exists("file.txt"))      # True/False
print(os.path.isfile("folder/"))       # False

shutil.copy("source.txt", "backup/")   # copy to folder
shutil.move("file.txt", "archive/")    # move + rename if needed
```

### Quick Summary – Most Used Patterns in One Place

```python
# Read all
with open("file.txt") as f:
    data = f.read()

# Read line by line (memory friendly)
with open("large.log") as f:
    for line in f:
        process(line)

# Write
with open("result.txt", "w") as f:
    f.write("Result\n")
    f.write(str(42) + "\n")

# Append log
with open("app.log", "a") as log:
    log.write("Error occurred\n")
```

Now you have **explanation + working mini-example** for almost every concept shown in the video.

Practice these 8–10 small snippets in your editor — especially the `with` + loop, `write` with `\n`, and binary copy. These patterns appear in almost every red team / automation script later.

Ready to move to the next module (`requests`)? Or want more file practice tasks first?
