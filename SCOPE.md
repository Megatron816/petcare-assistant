# 📌 Pet Care Assistant — Project Scope & Modules

## 1. Project Objective
Develop a full-featured Android application that helps pet owners manage pet health, diet, activity, grooming, reminders, and vet appointments.  
AI features will NOT be included in the main build (kept as future enhancement).

---

## 2. Key Modules (MVP)
The Minimum Viable Product will include:

### ✔ 1. Authentication
- User registration & login  
- Firebase email/password auth  
- Logout, forgot password  

### ✔ 2. Pet Profile Management
- Add/Edit/Delete pets  
- Upload pet photos  
- Store breed, age, weight, vaccination status  

### ✔ 3. Vaccination & Health Tracker
- Predefined vaccination schedule  
- Log completed vaccinations  
- Tag symptoms or issues  
- Store medical history  

### ✔ 4. Diet Planner (Rule-based)
- Recommended diet by breed, age, weight  
- Food suggestions from built-in database  
- Daily feeding reminders  

### ✔ 5. Grooming & Care Scheduler
- Bathing reminders  
- Nail trimming reminders  
- Medicine reminders  
- Custom reminders using WorkManager  

### ✔ 6. Activity Tracker
- Walk session tracking  
- Steps, distance, duration  
- Weekly & monthly charts  

### ✔ 7. Vet Locator & Appointments
- Google Maps view  
- Shows nearby vets (custom dataset allowed)  
- Let users book local appointments (no payment)

### ✔ 8. Community Feed
- Users can post images  
- Like & comment  
- Basic moderation (delete own posts)

### ✔ 9. Notifications
- Local notifications  
- FCM push notifications  

---

## 3. Out-of-Scope (NOT included in MVP)
The following features will NOT be implemented in MVP:

❌ AI diet recommendation  
❌ AI symptom checker  
❌ Wearable/BLE collar integration  
❌ In-app chat  
❌ Payment gateway  
❌ Marketplace for pet products  

These may be added in **Future Enhancements**.

---

## 4. Acceptance Criteria
- App should run on Android 11+  
- App must not crash on normal use  
- At least one pet must be successfully added & managed  
- Vaccination & grooming reminders should trigger notifications  
- Activity tracker should record a walk session  
- Vet locator must display minimum 5 dummy clinics  
- Community feed must allow posting photos  

---

## 5. Deliverables
- Android Studio project (Jetpack Compose + MVVM + Firebase + Room)  
- Complete documentation (SRS + UML + ERD + Use-case)  
- Test cases & demo video  
- Final presentation PPT  

---

## 6. Technologies Used
- Kotlin  
- Jetpack Compose  
- MVVM + Clean Architecture  
- Firebase Auth  
- Firebase Firestore  
- Firebase Storage  
- Room Database  
- Google Maps SDK  
- WorkManager  
- Retrofit (if using APIs)  
- Material 3  
