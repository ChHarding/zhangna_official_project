# Overview
This documentation provides an in-depth look at the Calorie Calculator App for developers. It covers the code structure, features, and guidelines for extending or modifying the app.

# Code Structure
- Modules
tkinter: For GUI creation.
pandas: To handle CSV data (future use).
rapidfuzz: For fuzzy matching food names (future use).
requests: For API requests to fetch nutritional data.

- Classes
CustomDialog: A dialog box to collect user input with sliders and radio buttons.
CalorieApp: The main application class inheriting from tk.Tk.

- Key Functions
calculate_bmr(): Calculates BMR and daily calorie needs based on user input.
search_food(meal): Fetches food data from the API and calculates calorie intake.
process_food_selection(food_item, index): Processes food details and updates calorie data.
update_calories_display(): Updates the GUI with current calorie data and the progress ring.


# Dependencies
- Python Version: 3.9+
- Required Libraries:
tkinter
pandas
rapidfuzz
requests

# Development Guidelines
- API Key Configuration
Replace the self.api_ninjas_key variable with your own API key.

- Adding New Features
Macronutrient Breakdown: Extend process_food_selection() to update macronutrient labels dynamically.
Data Persistence: Use pandas to log meals into a CSV file.

- Error Handling
Add try-except blocks around API requests and user input parsing to ensure robust error handling.

- UI Enhancements
Add icons for meal buttons to improve aesthetics.
Include tooltips for a better user experience.

# File Organization
Main Application: calorie_app.py
Dependencies: Installed via pip.

# Future Enhancements
User Accounts: Allow users to save their data.
Offline Mode: Use a local database to store food nutritional data.
Integration with Fitness Trackers: Sync calorie burn data from wearable devices.
