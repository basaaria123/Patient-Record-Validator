# 🏥 Patient Record Validator

## 📌 Overview

The Patient Record Validator is a Python-based system designed to validate, process, and organize patient data records. It ensures that all entries meet defined rules for correctness, completeness, and format.

The application classifies records into **valid** and **invalid**, provides detailed error categorization, and visualizes the results for better analysis.

---

## ⚙️ Features

### ✅ Field Validation
Validates required fields:
- ID  
- Name  
- Age  
- Phone  

### 🔍 Data Integrity Checks
- Age must be numeric and between **0–120**  
- Phone number must be a **10-digit number**  
- Name must contain only **alphabets and spaces**  

### 🔁 Duplicate Detection
Identifies duplicate IDs using efficient **set-based lookup**

### ⚠️ Custom Exception Handling
Errors are categorized into:
- Missing Field  
- Invalid Age  
- Invalid Name  
- Invalid Phone  
- Format Error  
- Duplicate ID  

### 📊 Data Visualization
Generates a **bar graph** comparing:
- Valid records  
- Invalid records  

### 📋 Structured Output
- Displays results in **clean tabular format**  
- Improves readability for analysis and debugging  

---

## 🛠️ Technologies Used

- Python 3  
- Matplotlib (for visualization)  

---

## 📁 Project Structure
##🧾 Input Format

Each record must follow:
ID:<number>,Name:<text>,Age:<number>,Phone:<10-digit number>

### Example:
ID:101,Name:Rahul,Age:25,Phone:9876543210


## ▶️ How to Run

1. Install Python (3.x recommended)

2. Install dependencies:
```bash
pip install matplotlib
Run the program:
python main.py
```

## 📤 Sample Output
✅ Valid Records
ID      Name                Age   Phone
--------------------------------------------------
401     Arun Kumar          30    9123456789

❌ Invalid Records
Record                                                      Error Type         Message
--------------------------------------------------------------------------------------------------------------
ID:431,Name:Test123,Age:30,Phone:9555555555              Invalid Name       Invalid Name
INVALID DATA                                             Format Error       Completely invalid record

---

## 📊 Graph Output

Displays a bar chart showing:
- ✔ Number of valid records  
- ✖ Number of invalid records  

---

## 📏 Validation Rules

| Field  | Rule |
|--------|------|
| ID     | Must be unique |
| Name   | Alphabets and spaces only |
| Age    | Integer between 0–120 |
| Phone  | Exactly 10 digits |

---

## 🚀 Advantages

- Improves data accuracy and reliability  
- Efficient duplicate detection using sets  
- Modular and easy to extend  
- Clear error classification  

---

## ⚠️ Limitations

- Works only with predefined string format  
- No database integration  
- Console-based (no GUI)  

---

## 🔮 Future Enhancements

- Add email validation 📧  
- Integrate database (MySQL / SQLite) 🗄️  
- Build GUI interface 🖥️  
- Export results to CSV/Excel 📁  
- Develop API support 🌐  

---

## 🧠 Conclusion

This project demonstrates the application of **data validation, exception handling, and structured processing** to ensure reliable and accurate data management—an essential requirement in real-world systems such as healthcare.

---

## 👤 Author

- Your Name  

---

## 📜 License

This project is intended for **educational purposes**.
