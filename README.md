# Weight Tracker App

Welcome to the Weight Tracker App repository! This Android application helps users track their daily weight entries and set goal weights.

## Features

- **User Authentication**: Allows users to log in or create a new account.
- **Weight Tracking**: Enables users to enter their daily weight and view their weight history.
- **Goal Setting**: Users can set a goal weight to track their progress.
- **SMS Notifications**: Provides optional SMS notifications for important updates.
- **Persistent Storage**: Uses SQLite database to store user information and weight entries.

## Screenshots

## Technologies Used

- Java
- Android SDK
- SQLite Database
- RecyclerView

## Setup Instructions

1. **Clone the repository**

2. **Open in Android Studio**
- Open Android Studio and select "Open an existing Android Studio project"
- Navigate to the cloned repository and select the `weight` directory.

3. **Run the app**
- Connect an Android device or use an emulator.
- Click on the "Run" button in Android Studio to install the app on your device/emulator.

## How to Use

- **Login**: Enter your username and password to log in.
- **Create Account**: If it's your first time, create a new account with a username and password.
- **Weight Entry**: Add your weight for the day and save it.
- **Goal Setting**: Set a goal weight from the main screen to track your progress.
- **SMS Notifications**: Enable SMS notifications for updates.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/your-feature`)
6. Create a new Pull Request

## Reflection

1. Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?
   - The requirements for this application were that the user needed to be able to login by using a username and password. It would check against it's database to see if the account existed, if it did not it would create the entry. The database would then create variables for this account and save the users specific data. The application prompts the user for SMS permissions, if they select yes, it will send an SMS message if they acheive their goal weight. The user needs to be able to set a goal weight, and add entries of current weights into a grid to track their progress. The entries should contain the weight and a date to track. The entries also need to able to deleted and modified. 
2. What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
  - The screens required for this application are the login screen, the SMS permissions screen, the home screen where the user enters their data. I focused on keeping the UI simple and clear, using high contrast colors and sticking to a color scheme. I also kept the font scheme coherent with easy to read fonts. I designed my screens to be read from left to right and top to bottom, as this is the standard format the target audience would use to read. My thought is that the user would have a single flow of actions to guide them subconciously through the entire application.
3. How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?
  - After conducting all the research and understanding the requirements, I started by brainstorming all the scripts I would need to interact with all the objects in the IDE. I went with a modular approach and each object is scripted so if another developer would pick up the files, they should have a decent understanding of what is happening and why. I also made sure the nomenclature was clear and each item described its function.
4. How did you test to ensure your code was functional? Why is this process important, and what did it reveal?
- Testing was super important to reveal any flaws in my design and code. I started by testing each object at its miniumum and maximum operating values to confirm my boundaries worked correctly. I checked to see if I denied SMS permissions that I would not be able to receive SMS notifications from the program. I tested entering goal weights, and weight entries under the goal to ensure notifications appeared. I tested modifying weight entries along with deleting them. I frequently closed the application during certain tasks to ensure the data saved and data was not lost.
5. Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?
 - I ran into some issues when programming the SMS notification and permissions. I was getting interesting results at first where the notification wouldn't appear. I created more isolated scripts for these events and my problems became clear. This also allowed me to make changes quicker. 
6. In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
 - The logic behind filling in the database and grid on the screen was something that I felt natural doing. This is something I have been working with in another class and a similar scenario at work. 

