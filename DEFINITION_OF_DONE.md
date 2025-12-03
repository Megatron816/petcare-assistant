# ✔ Success Criteria and Definition of Done (DoD)

## 1. Project Success Criteria
These are measurable outcomes that must be achieved:

1. The application must run smoothly on Android 11 and above.
2. Users must be able to create an account, log in, and manage their profile.
3. Users must be able to add, edit, and delete pets.
4. Vaccination reminders must trigger a local notification.
5. Diet planner must generate rule-based suggestions based on age, weight, breed.
6. Walk activity tracker must record steps, time, and distance.
7. Vet locator must display at least 5 clinics (dataset-based or map-based).
8. Community feed must allow posting photos with captions.
9. All data must sync with Firestore and also work offline using Room.
10. App must not crash during normal use (at least 20 test cases performed).

---

## 2. Feature-level Acceptance Criteria (per module)

### ✔ Authentication
- User can register and log in using Firebase.
- Error messages shown for invalid credentials.
- User stays logged in until logout (Firebase session persistence).

### ✔ Pet Management
- Add/Edit/Delete operations must work.
- Photos stored in Firebase Storage.
- Basic validations (name, breed, weight must not be empty).

### ✔ Reminders & Notifications
- WorkManager triggers reminders on exact time.
- Notification works even after app is closed.

### ✔ Activity Tracker
- Step counter updates in real time.
- Walk session can be started/paused/stopped.

### ✔ Vet Locator
- Vet locations load on map or list.
- Clicking on clinic opens details screen.

---

## 3. Definition of Done (DoD)
A feature is considered *DONE* only when:

1. **Code Completed**  
   - All logic implemented  
   - No TODOs left

2. **UI Completed**  
   - UI matches the mockups  
   - Responsive for multiple screen sizes

3. **Integrated with Architecture**  
   - Follows MVVM & Clean Architecture  
   - ViewModel + Repository implemented

4. **Testing**  
   - Unit tests written (where applicable)  
   - Feature manually tested on device/emulator  
   - No major bugs remain

5. **Documentation Updated**  
   - README updated (if needed)  
   - API or module documentation updated  
   - Screenshots added (if UI changed)

6. **Peer Review / Self-review**  
   - Code reviewed for style, structure, naming  
   - Passed review checklist

7. **Merged Successfully**  
   - PR approved  
   - Branch merged to `dev` (not directly to `main`)

---

## 4. Project Completion Criteria
The project is considered fully complete when:

- All modules in the SRS are implemented.
- All Success Criteria are met.
- DoD is applied to each feature.
- Full documentation (SRS, ERD, UML, PPT) is submitted.
- Final APK + source code uploaded to GitHub.
