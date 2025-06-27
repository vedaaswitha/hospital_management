
# 🏥 Hospital Management System (C Console Application)

A simple and efficient console-based Hospital Management System implemented in C.  
Designed to help manage patient records using a stack data structure and a clean terminal interface.  
Built as a part of a CS-102 project.

---

## 🔐 Features

### 🧑‍⚕️ User Authentication
- User registration with username and password (DOB as password)
- Secure login (3 attempts max)

### 🗂 Patient Record Management
- Add new patient records
- View all records sorted by age (Bubble Sort)
- Search records by first name (Linear Search)
- Update existing records
- Delete the last added record (LIFO stack behavior)

### ✅ Data Validation
- Validates name, gender, and input types
- Sanitized input for reliability

### 🖥 User Interface
- Menu-driven and console-based
- Clear formatting and navigation

---

## 🧱 Technical Details

### 📦 Data Structures
- Stack (array-based) with a maximum size of 10
- Patient struct:

```c
typedef struct patient {
    int age;
    char gender;
    char first_name[20];
    char last_name[20];
    char address[30];
    char phone[15];
    char problem[50];
    char doctor[20];
} patient;
```

### 🧠 Algorithms
- **Bubble Sort** – Sort patients by age
- **Linear Search** – Search by first name

### 🔑 Core Functions
- `add_record()` – Add new patient
- `view_record()` – Show all patients
- `search_record()` – Search by name
- `update_record()` – Edit record
- `delete_record()` – Remove last patient

---

## ⚙️ How to Compile and Run

### 🪟 On Windows
```bash
gcc hospital_management.c -o hospital_management
./hospital_management
```

---

## 📋 Usage Instructions

### 📝 Registration
- Enter a username and a password (DOB)

### 🔓 Login
- You have 3 attempts to log in with your credentials

### 🩺 Main Menu Options
1. Add new patient record  
2. View all records (sorted by age)  
3. Search patient by first name  
4. Update existing record  
5. Delete last added record  
6. Exit  

---

## 🧪 Limitations
- No file/database storage (data is in-memory only)
- Max 10 records due to fixed stack size
- Uses `conio.h` and `windows.h` – Windows-only
- Basic error handling

---

## 🚀 Future Enhancements
- Persistent storage using file system
- MySQL or SQLite integration
- Increased record capacity with linked list or dynamic array
- Cross-platform support (Linux, MacOS)
- Appointment and billing modules

---

## 👥 Contributors
Group 4 – CS-102 Project
