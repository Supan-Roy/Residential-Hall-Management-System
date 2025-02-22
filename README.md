# Residential Hall Management System

This is a simple C project for managing a residential hall system. It allows administrators to manage student records, view maintenance requests, and more. Students can also access their information, view hostel rules, and check the food menu.

## Features

### Admin Features:
1. **Add New Student**: Add a new student to the residential hall system.
2. **Update Student Information**: Modify existing student details (e.g., room number, phone number).
3. **View Student Details**: Check the details of a specific student.
4. **View All Students**: Display a list of all students in the system.
5. **Remove Student**: Delete a student's record from the system.
6. **View Maintenance Requests**: Check maintenance requests submitted by students.

### Student Features:
1. **View Personal Information**: Students can view their own details.
2. **View Hostel Rules**: Display the rules and regulations of the hostel.
3. **View Food Menu**: Check the weekly food menu.
4. **Request Maintenance**: Submit maintenance requests for their room.

## How to Use

1. **Admin Login**:
   - Username: `Admin`
   - Password: `1234`
   - After logging in, the admin can access the main menu to manage student records and view maintenance requests.

2. **Student Login**:
   - Students can log in using their hostel ID and name.
   - After logging in, students can view their personal information, hostel rules, food menu, and submit maintenance requests.

## Code Structure

- **Main Functions**:
  - `main()`: Entry point of the program.
  - `menu()`: Displays the main menu for admin.
  - `reg_user()`: Displays the menu for students.
  
- **Student Management Functions**:
  - `new_entry()`: Adds a new student to the system.
  - `edit()`: Updates student information.
  - `see()`: Displays details of a specific student.
  - `view_list()`: Lists all students in the system.
  - `erase()`: Removes a student from the system.

- **Utility Functions**:
  - `welcome_message()`: Displays a welcome message.
  - `rules()`: Displays hostel rules.
  - `food_menu()`: Displays the weekly food menu.
  - `maintenance()`: Allows students to submit maintenance requests.
  - `maintenance_view()`: Allows admin to view maintenance requests.

## How to Compile and Run

1. **Compile the Code**:
   ```bash
   gcc -o hall_management hall_management.c
   ```

2. **Run the Program**:
   ```bash
   ./hall_management
   ```

## Files Used

- `record.dat`: Stores student records.
- `maintenance.txt`: Stores maintenance requests submitted by students.
- Hostel-specific files (`BH-1.dat`, `BH-2.dat`, etc.): Store hostel-specific student IDs.

## Notes

- Ensure that the `record.dat` and `maintenance.txt` files are present in the same directory as the executable.
- The program uses simple file handling to store and retrieve data.
