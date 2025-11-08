 # OTUS Finance 🦉

A cross-platform personal finance management application built with .NET MAUI and C#. Track expenses, monitor spending habits, and maintain budget control across Android, iOS, macOS, and Windows platforms.

![OTUS Finance Logo](OtusFinance/Resources/Images/logo.png)

## 📋 Table of Contents
- [Features](#features)
- [Screenshots](#screenshots)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Key Learnings](#key-learnings)
- [Future Enhancements](#future-enhancements)
- [Contact](#contact)

## ✨ Features

### User Authentication
- Secure signup and login system
- Password management and account settings
- User session management

### Transaction Management
- Log expenses and income with categorization
- Transaction categories include:
  - Housing and Utilities
  - Food and Drinks
  - Travel
  - Income
  - Other Expenses
- Date-based transaction tracking
- Complete transaction history view

### Financial Insights
- **Dashboard**: Real-time overview of financial activity
  - Line chart visualization of income vs. expenses
  - Recent transaction feed
  - Monthly spending summary
- **Overview Page**: Visual spending analysis
  - Donut chart breakdown by category
  - Top spending category identification
  - Color-coded category legend
- **Budget Management**: Set and track monthly spending caps

### Data Visualization
- Interactive charts using Microcharts library
- Line charts for trend analysis
- Donut charts for category distribution
- Real-time data updates

## 📸 Screenshots
<img width="1002" height="477" alt="Screenshot 2024-05-06 201820" src="https://github.com/user-attachments/assets/8287f074-2cd2-4f59-b879-8f91c90b75f0" />
<img width="1009" height="474" alt="Screenshot 2024-05-06 201840" src="https://github.com/user-attachments/assets/a3ce830b-ff52-473f-83a4-acbf362cd868" />
<img width="1005" height="472" alt="Screenshot 2024-05-06 201935" src="https://github.com/user-attachments/assets/5dcac52f-6c81-42f7-9ab5-e825440ab868" />
<img width="1003" height="474" alt="Screenshot 2024-05-06 205913" src="https://github.com/user-attachments/assets/e3a58d25-3769-4ea1-9f8e-1a7e8822d22e" />
<img width="1063" height="567" alt="Screenshot 2024-05-06 202226" src="https://github.com/user-attachments/assets/b449312f-c416-40f2-b76c-56f0b17120c6" />
<img width="1060" height="565" alt="Screenshot 2024-05-06 202246" src="https://github.com/user-attachments/assets/0b6525d1-f7dc-4004-bfcf-546553a4e0cf" />

### Landing & Authentication
- Clean, modern landing page with branding
- Intuitive login and signup flows

### Dashboard
- At-a-glance financial summary
- Visual expense tracking
- Quick access to recent transactions

### Reports & Analytics
- Comprehensive transaction history
- Easy expense logging interface
- Detailed spending breakdowns

## 🛠 Tech Stack

**Framework & Language:**
- .NET 8.0
- C# 
- .NET MAUI (Multi-platform App UI)

**Database:**
- SQLite with SQLite-net-pcl
- Asynchronous database operations

**Data Visualization:**
- Microcharts.Maui
- SkiaSharp for custom graphics

**Platforms:**
- Android (API 21+)
- iOS (11.0+)
- macOS Catalyst (13.1+)
- Windows (10.0.17763.0+)

**Key Dependencies:**
```xml
- Microsoft.Maui.Controls (8.0.21)
- sqlite-net-pcl (1.9.172)
- Microcharts.Maui (1.0.0)
- SkiaSharp.Views.Maui.Controls (3.0.0)
```

## 🚀 Getting Started

### Prerequisites
- Visual Studio 2022 (v17.8+) with .NET MAUI workload
- .NET 8.0 SDK
- For mobile development:
  - Android SDK (for Android deployment)
  - Xcode (for iOS/macOS deployment)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/otus-finance.git
   cd otus-finance
   ```

2. **Restore NuGet packages**
   ```bash
   dotnet restore
   ```

3. **Build the solution**
   ```bash
   dotnet build
   ```

4. **Run the application**
   - Open `OtusFinance.sln` in Visual Studio
   - Select your target platform (Android, iOS, Windows, etc.)
   - Press F5 or click the Run button

### First-Time Setup
1. Launch the application
2. Click "Signup" on the landing page
3. Create an account with username and password
4. Log in with your credentials
5. Set your monthly spending cap in Settings
6. Start logging transactions!

## 📁 Project Structure

```
OtusFinance/
├── Database/
│   └── LocalDB.cs                 # SQLite database operations
├── Models/
│   ├── User.cs                    # User data model
│   └── Transactions.cs            # Transaction data model
├── Pages/
│   ├── LandingPage.xaml/.cs       # Entry point
│   ├── LoginPage.xaml/.cs         # Authentication
│   ├── SignupPage.xaml/.cs        # User registration
│   ├── DashboardPage.xaml/.cs     # Main dashboard
│   ├── AccountReport.xaml/.cs     # Transaction logging
│   ├── OverviewPage.xaml/.cs      # Spending analytics
│   └── AccountSettings.xaml/.cs   # User settings
├── Resources/
│   ├── Images/                    # App images and icons
│   ├── Styles/                    # XAML styling resources
│   └── Fonts/                     # Custom fonts
└── Platforms/                     # Platform-specific code
```

## 🎓 Key Learnings

### Technical Skills Demonstrated

**Cross-Platform Development:**
- Built a single codebase that runs on 4+ platforms
- Implemented platform-specific features and optimizations
- Managed responsive UI across different screen sizes

**Database Management:**
- Designed normalized database schema
- Implemented async/await patterns for data operations
- Created CRUD operations with proper error handling
- Managed data persistence across sessions

**UI/UX Design:**
- Created an intuitive, modern interface using XAML
- Implemented navigation flows with Shell architecture
- Designed consistent visual language across pages
- Added data visualization components

**State Management:**
- Managed application state with static UserData class
- Implemented data binding with MVVM concepts
- Handled lifecycle events and page navigation

**Problem-Solving:**
- Debugged database connection issues
- Optimized chart rendering performance
- Implemented input validation and error handling

## 🔮 Future Enhancements

### Planned Features
- [ ] Export transactions to CSV/PDF
- [ ] Budget alerts and notifications
- [ ] Recurring transaction support
- [ ] Multi-currency support
- [ ] Biometric authentication
- [ ] Cloud sync across devices
- [ ] Receipt photo attachments
- [ ] Advanced filtering and search
- [ ] Spending predictions using ML
- [ ] Dark mode refinements

### Technical Improvements
- [ ] Implement MVVM architecture with CommunityToolkit.Mvvm
- [ ] Add unit and integration tests
- [ ] Implement data encryption
- [ ] Add localization support
- [ ] Optimize database queries with indexing
- [ ] Implement data backup/restore


## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- OTUS branding and logo design
- Microcharts library for visualization components
- .NET MAUI community for documentation and support

---

*Built with 💚 using .NET MAUI*
