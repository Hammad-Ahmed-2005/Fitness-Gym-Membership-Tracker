# 🏋️ Fitness Gym Membership Tracker

A comprehensive C-based console application for managing gym memberships and tracking diet logs. Built as a Programming Fundamentals course project, this system demonstrates core C programming concepts including file handling, arrays, structures, and functions.

## 📖 About

This Gym Membership & Diet Logger is a terminal-based application designed to help gym administrators manage member information, track membership status, and maintain diet logs for their clients. The application provides an intuitive menu-driven interface for performing various administrative tasks.

## ✨ Features

- 👥 **Member Management**
  - Add new gym members
  - View member details
  - Update member information
  - Delete member records
  - Search members by ID or name

- 💳 **Membership Tracking**
  - Track membership start and end dates
  - Monitor membership status (active/expired)
  - Manage different membership types
  - Calculate membership duration

- 🍎 **Diet Logger**
  - Create personalized diet plans
  - Log daily meals and calorie intake
  - Track nutritional information
  - View diet history for members

- 💾 **File Handling**
  - Persistent data storage using file I/O
  - Automatic data saving
  - Data retrieval on program startup

## 🛠️ Technical Implementation

### Core Concepts Used

- **Structures**: Custom data types for members, memberships, and diet entries
- **Arrays**: Efficient data storage and management
- **Functions**: Modular code organization with dedicated functions for each operation
- **File Handling**: Reading from and writing to files for data persistence
- **Menu-Driven Interface**: User-friendly navigation system

### Data Structures

```c
struct Member {
    int id;
    char name[50];
    int age;
    char gender;
    char contact[15];
    // Additional fields
};

struct Membership {
    int memberId;
    char startDate[11];
    char endDate[11];
    char type[20];
    float fee;
};

struct DietLog {
    int memberId;
    char date[11];
    char meal[100];
    int calories;
};
```

## 📋 Prerequisites

- GCC Compiler (MinGW for Windows, GCC for Linux/Mac)
- C programming knowledge
- Terminal/Command Prompt access

## 🚀 Installation & Setup

### For Windows:

1. Clone the repository:
```bash
git clone https://github.com/Hammad-Ahmedd/Fitness-Gym-Membership-Tracker.git
```

2. Navigate to the project directory:
```bash
cd Fitness-Gym-Membership-Tracker
```

3. Compile the program:
```bash
gcc main.c -o gym_tracker.exe
```

4. Run the executable:
```bash
gym_tracker.exe
```

### For Linux/Mac:

1. Clone the repository:
```bash
git clone https://github.com/Hammad-Ahmedd/Fitness-Gym-Membership-Tracker.git
```

2. Navigate to the project directory:
```bash
cd Fitness-Gym-Membership-Tracker
```

3. Compile the program:
```bash
gcc main.c -o gym_tracker
```

4. Run the executable:
```bash
./gym_tracker
```

## 💻 Usage

Upon running the program, you'll be presented with a main menu:

```
=================================
  GYM MEMBERSHIP TRACKER
=================================
1. Add New Member
2. View All Members
3. Search Member
4. Update Member
5. Delete Member
6. Add Membership
7. View Memberships
8. Add Diet Log
9. View Diet Logs
10. Exit
=================================
Enter your choice: 
```

### Example Workflow:

1. **Adding a Member**: Select option 1 and enter member details
2. **Adding Membership**: Select option 6 and link it to a member ID
3. **Logging Diet**: Select option 8 to record daily meals
4. **Viewing Data**: Use options 2, 7, or 9 to view stored information

## 📁 Project Structure

```
Fitness-Gym-Membership-Tracker/
├── main.c              # Main program file
├── members.txt         # Member data storage
├── memberships.txt     # Membership records
├── diet_logs.txt       # Diet log entries
└── README.md           # Project documentation
```

## 🔍 Key Functions

- `addMember()` - Adds a new gym member to the system
- `viewMembers()` - Displays all registered members
- `searchMember()` - Searches for a member by ID or name
- `updateMember()` - Updates existing member information
- `deleteMember()` - Removes a member from the system
- `addMembership()` - Creates a new membership record
- `viewMemberships()` - Lists all membership details
- `addDietLog()` - Logs diet information for a member
- `viewDietLogs()` - Displays diet history
- `saveToFile()` - Persists data to files
- `loadFromFile()` - Retrieves data from files

## 🎓 Learning Outcomes

This project demonstrates proficiency in:

- ✅ Designing and implementing structures in C
- ✅ Working with arrays for data management
- ✅ Creating modular functions for code reusability
- ✅ Implementing file I/O operations
- ✅ Building menu-driven console applications
- ✅ Managing memory and data flow
- ✅ Implementing CRUD operations (Create, Read, Update, Delete)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Hammad-Ahmedd/Fitness-Gym-Membership-Tracker/issues).

### How to Contribute:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Course Information

- **Course**: Programming Fundamentals (PF)
- **Language**: C Programming
- **Concepts**: File Handling, Arrays, Structures, Functions

## 🐛 Known Issues

- Data validation could be enhanced
- No database integration (uses file-based storage)
- Limited error handling for edge cases

## 🔮 Future Enhancements

- [ ] Add payment tracking system
- [ ] Implement attendance tracking
- [ ] Add workout plan management
- [ ] Include progress tracking and analytics
- [ ] Add password protection for admin access
- [ ] Implement data backup and restore
- [ ] Create a graphical user interface (GUI)
- [ ] Add report generation features

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Hammad Ahmed**

- GitHub: [@Hammad-Ahmedd](https://github.com/Hammad-Ahmedd)
- Project Link: [Fitness-Gym-Membership-Tracker](https://github.com/Hammad-Ahmedd/Fitness-Gym-Membership-Tracker)

## 🙏 Acknowledgments

- Thanks to the Programming Fundamentals course instructors
- Inspired by real-world gym management systems
- C programming community for resources and support

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Contact through GitHub profile

---

**Note**: This project was created as part of a Programming Fundamentals course to demonstrate understanding of C programming concepts. It serves as a practical implementation of file handling, data structures, and modular programming principles.

---

⭐ Star this repository if you found it helpful!
