# IMADASSIGNMENT01
 . Setting Up the Project

I began by creating a new Android project in Android Studio with an Empty Activity template. Kotlin was selected as the programming language. The MainActivity.kt file was automatically created along with the activity_main.xml layout file.

2. Designing the User Interface (UI)

I designed the UI in the activity_main.xml file using the Layout Editor:

EditText: A text box was added for the user to input the time of day (e.g., “morning”, “afternoon”).

TextView: This displays the suggested meal.

Button (Suggest): When clicked, it processes the input and shows the meal suggestion.

Button (Reset): Clears both the input and the suggestion display.

All UI components were given meaningful IDs for reference in the Kotlin code.

3. Implementing Meal Suggestion Logic

In the MainActivity.kt file, I added functionality to respond to user input:

The app retrieves the input string using inputTime.text.toString().

I used if and when statements (a Kotlin feature similar to switch in other languages) to check the input.

Based on the input, the app displays meal suggestions taken from the Spur menu, such as:

Morning: Spur Ranch Breakfast

Mid-morning: Cheesy Garlic Roll

Afternoon: Spur Classic Burger

Mid-afternoon: Buffalo Wings

Dinner: T-Bone Steak

After dinner: Chocolate Brownie

4. Error Handling

To enhance usability, I added input validation:

If the user enters an invalid or empty string, a clear error message appears (e.g., "Invalid input. Please enter a valid time of day.").

This prevents confusion and keeps the app experience smooth and helpful.

5. Reset Button Functionality

The reset button uses inputTime.text.clear() and resultText.text = "" to clear both the input and output fields, allowing Hera to easily start over.

6. Testing the App

I tested the app on an Android Virtual Device (AVD) in the emulator:

Inputs like “morning”, “mid-afternoon”, and “after dinner” returned the correct Spur meal.

Invalid inputs like “xyz” or blank entries prompted appropriate error messages.

Conclusion

The app was created with the goal of making Hera’s mealtime choices easier and more fun. By combining Kotlin logic, Android UI design, and effective error handling, the app offers a clean and engaging experience tailored to her needs.
