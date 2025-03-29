# Quiz Management System in Java

## 📋 Description
A Java-based software system designed to manage quizzes effectively. It provides role-based login functionalities for **Admins** and **Students**. Admins can create and manage a quiz bank with multiple-choice questions (MCQs), while students can take randomly generated quizzes.

---

## ✨ Features

- Admins can add multiple MCQs with four options and a correct answer key to a `quiz.json` file.
- Admins can keep adding questions until they press `q` on the keyboard.
- Students can take a quiz with **10 random MCQs** selected from the quiz bank.
- Score is calculated based on correct answers.
- System provides feedback messages based on quiz performance.
- Role-based login (Admin and Student).

---

## 💠 Tools Used

- **IDE**: IntelliJ IDEA  
- **Build Tool**: Gradle

---

## 🚀 How to Run

### 1. Setup Project
- Clone the repository and open it in **IntelliJ IDEA**.
- Make sure **Gradle** is properly configured and all dependencies are resolved.

### 2. Prepare Resources

Create the following files in the `src/resources/` directory:

#### `users.json`
```json
[
  {
    "username": "admin",
    "password": "1234",
    "role": "admin"
  },
  {
    "username": "ali",
    "password": "1234",
    "role": "student"
  }
]
```

#### `quiz.json`
```json
[
  {
    "question": "Which is not part of system testing?",
    "option 1": "Regression Testing",
    "option 2": "Sanity Testing",
    "option 3": "Load Testing",
    "option 4": "Unit Testing",
    "answerkey": 4
  },
  {
    "question": "Which is whitebox testing technique?",
    "option 1": "Equivalent Partitioning",
    "option 2": "Boundary value testing",
    "option 3": "Decision table testing",
    "option 4": "Adhoc Testing",
    "answerkey": 3
  }
]
```

### 3. Run the Application
- Execute the **main class**.
- Use the following credentials:

> **Admin Login**  
> `username: admin`, `password: 1234`  
>  
> **Student Login**  
> `username: ali`, `password: 1234`

---

## 👩‍💼 Admin Functionalities

- Add SQA-related MCQs by entering the question, four options, and the correct answer key.
- Admin can continue to add questions until `q` is pressed.
- Minimum 30 questions should be added.

### Example:
```
System:> Enter your username  
User:> admin  
System:> Enter password  
User:> 1234  
System:> Welcome admin! Please create new questions in the question bank.

System:> Input your question  
Admin:> Which is not part of system testing?  
System: Input option 1:  
Admin: Regression Testing  
System: Input option 2:  
Admin: Sanity Testing  
System: Input option 3:  
Admin: Load Testing  
System: Input option 4:  
Admin: Unit Testing  
System: What is the answer key?  
Admin: 4  
System:> Saved successfully! Do you want to add more questions? (press s for start and q for quit)
```

---

## 🎓 Student Functionalities

- Attempt a 10-question multiple-choice quiz.
- Score and performance feedback provided instantly.
- Random questions may repeat if the quiz bank has few entries.
- Incorrect or invalid input counts as 0 marks.

### Example:
```
System:> Enter your username  
User:> ali  
System:> Enter password  
User:> 1234  
System:> Welcome ali to the quiz! We will throw you 10 questions. Each MCQ is worth 1 mark. No negative marking. Are you ready? Press 's' to start.

Student:> s

[Question 1] Which is not part of system testing?  
1. Regression Testing  
2. Sanity Testing  
3. Load Testing  
4. Unit Testing  
Student:> 4  

[Question 2] Which is whitebox testing technique?  
1. Equivalent Partitioning  
2. Boundary value testing  
3. Decision table testing  
4. Adhoc Testing  
Student:> 3
```

### Feedback Based on Score
- **8-10**: Excellent! You have got [marks] out of 10
- **6-7**: Good. You have got [marks] out of 10
- **3-5**: Very poor! You have got [marks] out of 10
- **0-2**: Very sorry, you are failed. You have got [marks] out of 10

```
System:> Quiz finished! Your score: 8/10  
Excellent! You have got 8 out of 10.  
Would you like to start again? Press 's' for start or 'q' for quit.
```

---

## 🎥 Demo Video

📺 [Click here to watch the demonstration](https://drive.google.com/file/d/1U2fotQTcmuZitHUgO2nnGj90F2JkHr6Q/view?usp=sharing)

---

## 📦 Author / Maintainer

*Ali Ahasan*

---

## 📆 Submission Checklist

- [x] Project uploaded to GitHub ✅
- [x] `.idea`, `.gradle`, `gradle`, and `build` folders/files added to `.gitignore` ✅
- [x] Project information documented in `README.md` ✅
- [x] Video recorded and linked in `README.md` ✅
