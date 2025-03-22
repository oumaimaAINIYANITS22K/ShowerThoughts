# 💭 ShowerThoughts – Phase 1 Documentation

## 👤 User Personas

Here are three detailed and well-documented user personas that represent different types of users for the ShowerThoughts app.

---

### 👤 Sara the Overthinker

- **Age:** 21  
- **Occupation:** University Student  
- **Tech Level:** Comfortable with web and mobile apps  
- **Goals:**
  - Dump her 2AM deep thoughts before forgetting them  
  - Track her emotional evolution through her thoughts  
- **Pain Points:**
  - Notes app is cluttered with to-dos and groceries  
  - Often forgets thoughts before finding something to write them down  
- **Behavior:**
  - Uses the app before bed daily  
  - Mostly tags thoughts as “🤔 Deep” or “💡 Genius”

---

### 👤 Tomi the Philosophical Barista

- **Age:** 26  
- **Occupation:** Part-time Barista, Part-time Poet  
- **Tech Level:** Moderate – prefers minimalist tools  
- **Goals:**
  - Capture poetic or quirky thoughts as writing inspiration  
  - Use randomizer feature for creative prompts  
- **Pain Points:**
  - Notes apps feel too formal  
  - Gets distracted easily while writing  
- **Behavior:**
  - Adds thoughts during daily commute  
  - Frequently uses the “Surprise Me” feature for fun

---

### 👤 Aino the Organized Oddball

- **Age:** 30  
- **Occupation:** UX Designer  
- **Tech Level:** High – advanced user  
- **Goals:**
  - Organize random ideas for future creative work  
  - Easily search and filter through tagged content  
- **Pain Points:**
  - Gets frustrated with untagged or unorganized notes  
- **Behavior:**
  - Always adds a tag  
  - Hides private thoughts using the “Mark as Private” option

---

## 📘 Use Cases

This section outlines the five primary use cases of the ShowerThoughts application.

---

### 🔹 Use Case 1: Add a New Thought

- **Use Case ID:** UC01  
- **Title:** Add a New Thought  
- **Actor:** User  
- **Preconditions:** User is on the “Add Thought” page  
- **Basic Flow:**
  1. User types a thought in the input field  
  2. User selects a tag from a dropdown (e.g. 🤔 Deep, 😂 Funny)  
  3. User checks “Mark as Private” (optional)  
  4. User clicks “Save”  
  5. Thought is stored in the database with a timestamp  
- **Postconditions:** The thought is saved and visible in the Thought List (unless marked private)  
- **Alternative Flow:**  
  - If the input field is empty, the system shows an error message and prevents submission

---

### 🔹 Use Case 2: View All Thoughts

- **Use Case ID:** UC02  
- **Title:** View All Thoughts  
- **Actor:** User  
- **Preconditions:** The user has previously submitted at least one thought  
- **Basic Flow:**
  1. User navigates to the “Thought List” page  
  2. App fetches all non-private thoughts from the database  
  3. Thoughts are displayed in chronological order  
- **Postconditions:** User can see all saved thoughts in a scrollable list  
- **Alternative Flow:**  
  - If no thoughts exist, app displays an empty state message like “Your brain’s still loading…”

---

### 🔹 Use Case 3: Filter Thoughts by Tag

- **Use Case ID:** UC03  
- **Title:** Filter by Tag  
- **Actor:** User  
- **Preconditions:** At least one thought exists with a tag (💡, 🤔, etc.)  
- **Basic Flow:**
  1. User opens the filter dropdown  
  2. User selects a tag (e.g., “😂 Funny”)  
  3. The system displays only thoughts with that tag  
- **Postconditions:** User sees a filtered list of thoughts  
- **Alternative Flow:**  
  - If no thoughts exist for that tag, app shows: “No thoughts here... try thinking funnier thoughts next time.”

---

### 🔹 Use Case 4: Random Thought Generator

- **Use Case ID:** UC04  
- **Title:** Surprise Me  
- **Actor:** User  
- **Preconditions:** At least one non-private thought is saved  
- **Basic Flow:**
  1. User clicks “Surprise Me”  
  2. The app randomly selects a public thought from the database  
  3. The selected thought is displayed in a popup or dedicated area  
- **Postconditions:** A random thought is shown  
- **Alternative Flow:**  
  - If no public thoughts exist, show a funny error:  
    > “Looks like your brain is on vacation today…”

---

### 🔹 Use Case 5: Delete Thought

- **Use Case ID:** UC05  
- **Title:** Delete Thought  
- **Actor:** User  
- **Preconditions:** User is viewing their list of thoughts  
- **Basic Flow:**
  1. User clicks the delete (🗑️) icon next to a thought  
  2. App asks for confirmation: “Delete this masterpiece?”  
  3. User confirms  
  4. App removes the thought from the database  
- **Postconditions:** Thought is no longer stored or visible  
- **Alternative Flow:**  
  - If user cancels the delete, the app takes no action

---
