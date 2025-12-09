# Mobile Zone

A Windows Forms desktop application for managing mobile phone inventory and customer information. Built with C# and .NET Framework 4.7.2.

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Database](#database)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## 🎯 About

Mobile Zone is a desktop application designed for managing mobile phone inventory and customer records. It provides a user-friendly interface for adding, viewing, and managing mobile phones and customer information in a retail or business environment.

This project was developed as part of **Year 1 Semester 3 Object Oriented Programming with C#** coursework.

## ✨ Features

- **User Authentication**: Secure login system
- **Customer Management**: Add, view, update, and delete customer records
- **Mobile Phone Management**: Manage mobile phone inventory with details
- **Data Viewing**: View all records in a tabular format
- **Database Integration**: SQL Server LocalDB for data persistence
- **Modern UI**: Windows Forms with intuitive navigation

## 🔧 Prerequisites

Before you begin, ensure you have the following installed:

- **Visual Studio 2017 or later** (or Visual Studio Code with C# extension)
- **.NET Framework 4.7.2** or higher
- **SQL Server LocalDB** (usually included with Visual Studio)
- **Windows OS** (Windows 7 or later)

## 📦 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/mobile-zone-2024.git
   cd mobile-zone-2024
   ```

2. **Open the solution**

   - Open `Mobile Zone.sln` in Visual Studio

3. **Database Setup**

   - The database files (`Mobile Zone.mdf` and `Mobile Zone_log.ldf`) are included in the project
   - Ensure SQL Server LocalDB is installed and running
   - Update the connection string in the source files if your database path differs
   - The default connection string is configured for LocalDB

4. **Build the project**
   - Press `F5` or go to `Build > Build Solution`
   - The application will compile and run

## 🚀 Usage

1. **Launch the application**

   - Run the executable from `bin/Debug/Mobile Zone.exe` or press `F5` in Visual Studio

2. **Login**

   - Enter your credentials on the login screen

3. **Navigate the application**

   - Use the Home screen to access different modules:
     - **Customer**: Manage customer records
     - **Mobile Phone**: Manage mobile phone inventory
     - **View**: View all records
     - **Logout**: Return to login screen

4. **Manage Data**
   - Add new records using the input fields
   - View existing records in the data grid
   - Update or delete records as needed

## 📁 Project Structure

```
mobile-zone-2024/
├── Customer.cs              # Customer management form
├── Customer.Designer.cs     # Customer form designer
├── Customer.resx            # Customer form resources
├── Home.cs                  # Main home/dashboard form
├── Home.Designer.cs         # Home form designer
├── Home.resx                # Home form resources
├── login.cs                 # Login form
├── login.Designer.cs        # Login form designer
├── login.resx               # Login form resources
├── MobilePhone.cs           # Mobile phone management form
├── MobilePhone.Designer.cs  # Mobile phone form designer
├── MobilePhone.resx         # Mobile phone form resources
├── View.cs                  # View records form
├── View.Designer.cs         # View form designer
├── View.resx                # View form resources
├── Program.cs               # Application entry point
├── App.config               # Application configuration
├── Mobile Zone.csproj       # Project file
├── Mobile Zone.sln          # Solution file
├── Mobile Zone.mdf          # SQL Server database file
├── Mobile Zone_log.ldf      # SQL Server log file
├── Properties/              # Application properties
│   ├── AssemblyInfo.cs
│   ├── Resources.Designer.cs
│   ├── Resources.resx
│   ├── Settings.Designer.cs
│   └── Settings.settings
└── Resources/               # Application resources (images, icons)
    ├── customer_3126647.png
    ├── document_5430673.png
    ├── logout_1828479.png
    ├── MOBILE-1-removebg-preview.png
    ├── smartphone_7234603.png
    └── square-x_10456583.png
```

## 🛠️ Technologies Used

- **C#** - Programming language
- **.NET Framework 4.7.2** - Framework
- **Windows Forms** - UI framework
- **SQL Server LocalDB** - Database
- **ADO.NET** - Data access technology
- **Visual Studio** - Development environment

## 💾 Database

The application uses **SQL Server LocalDB** with the following structure:

- **Database File**: `Mobile Zone.mdf`
- **Log File**: `Mobile Zone_log.ldf`
- **Connection**: LocalDB instance
- **Tables**:
  - `CTBL` - Customer table
  - Additional tables for mobile phone inventory

### Database Connection

The connection string is configured in the source code. Default connection:

```
Data Source=(LocalDB)\MSSQLLocalDB;AttachDbFilename="[Path]\Mobile Zone.mdf";Integrated Security=True;Connect Timeout=30
```

**Note**: Update the connection string path in the source files to match your local database location.

## 📸 Screenshots

_Add screenshots of your application here to showcase the UI and features._

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

- **Development Team** - Year 1 Semester 3 Object Oriented Programming with C#

## 🙏 Acknowledgments

- Built as part of Year 1 Semester 3 Object Oriented Programming coursework
- Icons and images from various sources (see Resources folder)

---

**Note**: This is an academic project. For production use, consider implementing additional security measures, error handling, and database connection management best practices.
