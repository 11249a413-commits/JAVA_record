# Java Lab Record Programs

This repository contains beginner-friendly Java lab programs for the requested topics.

## Programs included

| No. | Folder | Program |
|---|---|---|
| 4(a) | `04_Inheritance` | Handling inheritance in Java |
| 5(a) | `05_Thread_Creation` | Creation of a thread in Java applications |
| 5(b) | `06_Multithreading` | Multithreading using multiple threads |
| 6(a) | `07_Predefined_Exceptions` | Handling predefined exceptions |
| 6(b) | `08_User_Defined_Exception` | Handling a user-defined exception |
| 7 | `09_File_Operations` | File creation, writing and reading |
| 8(a) | `10_Applet` | Simple applet program (legacy syllabus example) |
| 8(b) | `11_Color_Palette` | AWT color palette |
| 9(a) | `12_Layouts` | Handling layouts in Java |
| 9(b) | `13_Swing_Controls` | Handling Swing controls |
| 10(a) | `14_Database_Connectivity` | JDBC backend connectivity and data retrieval |

Each folder contains source code and a short `OUTPUT.txt` or `NOTES.md` where useful.

## Requirements

- JDK 8 or later for most programs.
- JDK 8 is recommended if your lab specifically requires running Applets.
- Applets are obsolete and were removed from modern Java/browser workflows. The applet source is included for syllabus/record purposes; it will not run directly with JDK 26.
- JDBC example uses MySQL. Install MySQL Server and add MySQL Connector/J to the classpath.

## Compile and run a normal Java program

Open Command Prompt or the VS Code terminal in the program folder:

```bash
javac ProgramName.java
java ProgramName
```

For AWT/Swing programs, run them on a desktop with a graphical display.

## JDBC setup

1. Create a database and table using `14_Database_Connectivity/schema.sql`.
2. Edit `DBConnection.java` and enter your MySQL username/password.
3. Download MySQL Connector/J from the official MySQL website.
4. Compile and run with the connector JAR on the classpath.

Windows example (replace the JAR path with your actual path):

```bat
javac -cp ".;mysql-connector-j-8.x.x.jar" *.java
java -cp ".;mysql-connector-j-8.x.x.jar" RetrieveStudents
```

Do not upload real database passwords to a public GitHub repository. Use a local password or environment variable.

## Upload to GitHub

1. Create a new GitHub repository, for example `Java-Lab-Record`.
2. Extract this ZIP file.
3. Open the extracted `Java_Lab_Record` folder.
4. Upload the folders and `README.md` to your repository, or use Git:

```bash
git init
git add .
git commit -m "Add Java lab record programs"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/Java-Lab-Record.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username and use your actual repository URL.
