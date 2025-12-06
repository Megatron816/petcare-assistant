Project: PetCare Assistant App
Version 1.1
Date: 2025
1. Introduction
   
1.1 Purpose
The PetCare Assistant App helps pet owners manage all aspects of pet care, including profiles, health records, reminders, activity tracking, shopping lists, and nearby services.
This SRS defines the functional and non-functional requirements for the app.

1.2 Scope
The PetCare Assistant App provides a centralized platform for pet owners to:
Register/login using Firebase Authentication
Create and manage pet profiles
Track vaccinations, medical history, and health records
Schedule reminders for feeding, grooming, vaccination, etc.
Log daily activities and view analytics
Locate nearby vets and pet stores
Maintain a shopping list
Configure app settings (theme, notifications)
The system is developed for Android devices using MVVM architecture.

1.3 Definitions & Acronyms
Term	Meaning
SRS	Software Requirements Specification
DB	Database
UI	User Interface
API	Application Programming Interface
MVVM	Model View ViewModel
CRUD	Create, Read, Update, Delete
------------------------------------------------------------------------------------------------------------------------------
2. Overall Description
2.1 User Types
Pet Owner – primary user of the application
(No additional roles in this version)

2.2 Product Features (Summary)
Authentication (Login/Signup/Forgot Password)
Pet profile management
Reminders & notifications
Health record tracking
Daily activity tracking
Nearby pet services (Maps + Places API)
Shopping list
Settings & app preferences

2.3 Constraints
Requires internet for authentication and maps
Notifications limited by device OS restrictions
Google Maps API requires a valid key

2.4 Assumptions
Users own at least one pet
Users have basic smartphone knowledge
----------------------------------------------------------------------------------------------------------------------------------
3. System Features (Functional Requirements)
3.1 Authentication Module (Firebase Auth)
FR1: User shall sign up using email & password
FR2: User shall log in using email & password
FR3: User shall reset password using email
FR4: Authentication state shall persist until logout
3.2 Pet Profile Module (Local DB)
FR5: User shall add a pet profile (name, breed, age, photo, etc.)
FR6: User shall edit pet profile details
FR7: User shall delete a pet profile
FR8: User data shall be stored locally using Room Database
3.3 Reminder Module
FR9: User can create reminders for feeding, grooming, vaccination
FR10: App shall trigger notifications at scheduled time
FR11: Notifications must fire even if app is closed (using WorkManager)
3.4 Health Records Module
FR12: User can add veterinary visit details
FR13: User can store vaccination records
FR14: User can maintain medication & dosage history
FR15: All health data stored locally using Room DB
FR16: User can view health history timeline
3.5 Activity Tracker Module
FR17: User can log activities (walk, play, diet, bath, etc.)
FR18: User can view daily/weekly/monthly logs
FR19: App shall generate basic analytics (charts/trends)
3.6 Nearby Services Module (Google Maps + Places API)
FR20: App shall show nearby pet services:
Veterinarians
Pet stores
Grooming centers
FR21: App shall show map view with markers
FR22: App shall show service details (rating, contact, directions)
3.7 Shopping List Module
FR23: User can add items to the shopping list
FR24: User can mark items as purchased
FR25: User can delete items
FR26: Shopping list stored in Room Database
3.8 Settings Module
FR27: User can switch between Light Mode / Dark Mode
FR28: User can enable/disable notifications
FR29: User can update their account details
FR30: User can log out
----------------------------------------------------------------------------------------------------------------------------
4. Non-Functional Requirements (NFRs)
4.1 Performance Requirements
NFR1: Dashboard should load in under 2 seconds
NFR2: Reminders must trigger within ±5 seconds of scheduled time

4.2 Security Requirements
NFR3: All authentication handled via Firebase Auth
NFR4: Local DB encrypted using SQLCipher (optional)

4.3 Usability Requirements
NFR5: UI should follow Material 3 guidelines
NFR6: Navigation should require no more than 3 taps to reach core features

4.4 Reliability Requirements
NFR7: No crash allowed under normal usage
NFR8: Notifications must work even after device reboot

4.5 Compatibility Requirements
NFR9: App must support Android API Level 24 and above
------------------------------------------------------------------------------------------------------------------------------------------
5. External Interface Requirements
5.1 User Interface
Material 3 theme
Bottom navigation bar
Clean card-based UI
Dark/Light mode support

5.2 Software Interfaces
Firebase Authentication
Google Maps API
Google Places API
Room Database
WorkManager
Jetpack Components (Navigation, LiveData, ViewModel, DataStore)
------------------------------------------------------------------------------------------------------------------------------------
6. System Models (High-Level)
6.1 Use Case Diagram (Description)
User manages pets
User manages reminders
User tracks health
User logs activities
User uses map location services
User manages shopping list
User changes settings
(I will generate the diagram image for you upon request.)

6.2 ER Diagram (Description)
Tables:
User
Pet
HealthRecord
Reminder
ActivityLog
ShoppingItem
(ER diagram image can be generated upon request.)

7. Future Enhancements
Cloud sync of all pet data
Multi-pet household sharing
AI-based pet health insights
Pet vaccination certificate generator

8. Conclusion

This document outlines all requirements for the first version of the PetCare Assistant App.
It will guide design, development, and testing throughout the project.
