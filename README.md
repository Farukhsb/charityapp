# CharityApp

An Android application for charity management and donations.

## Project Structure

The application is organised using logical, feature-based package grouping within Android Studio.  
This structure separates UI components, business logic, and data models to improve maintainability and scalability.  
The layout below represents the **conceptual organisation of the code**, rather than the raw folder structure displayed on GitHub.

```text
com.kodemakers.charity/
├── activities/
│   ├── authentication/      # LoginActivity, SignUpActivity, ForgotPasswordActivity
│   ├── donor/               # MainActivity, CharityDetailsActivity, DonationActivity
│   ├── charity/             # AddNewStoryActivity, UpdateCharityDetailsActivity, AddStaffActivity
│   ├── user/                # ProfileActivity, AccountDetailsActivity, UsersListActivity
│   ├── content/             # StoriesActivity, PlayVideoActivity, AddVideoFeedActivity
│   └── common/              # SplashActivity, NotificationActivity, IntroSteppersActivity
├── adapter/                 # RecyclerView adapters
├── model/                   # Data models (User, Charity, Donation)
├── service/                 # Business logic & API services
├── custom/                  # Custom UI components
├── utilies/                    # Fonts, helpers, extensions
└── CharityApp.java          # Application class
```

## Technical Details
- **Language**: Java (100%)
- **Package**: `com.kodemakers.charity`

##  Quick Start

### Prerequisites
- Android Studio
- Firebase account

### Installation
 Clone the repository:
   ```bash
   git clone https://github.com/JstMagic/charityapp.git
   cd charityapp
```

1. Firebase Setup:
   · Create a Firebase project
   · Add Android app with package: com.kodemakers.charity
   · Download google-services.json
   · Replace the file in app/ directory
2. Build and Run:
   ```bash
   # Open in Android Studio
   # Click Run → Run 'app'
   ```

Features (Based on Activity Names)

- User Authentication: Login, SignUp, ForgotPassword
- Charity Management: Add stories, videos, staff, update details
- Donation System: Process and track donations
- User Profiles: Contributor and account management
- Content Management: Stories, videos, onboarding
- Admin Features: User and staff listings
- Notifications: In-app notifications system

 Important Notes
 
- Update dependencies for current Android versions
- Requires Firebase configuration
- Contains both donor and admin interfaces

 Links

· Repository: https://github.com/JstMagic/charityapp
