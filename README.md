# 📱 Flutter Challenge: Staff App

Welcome to the Flutter challenge! Your goal ist to build an Android App for an Event Supervisor listing the staff that has been assigned to him.

The App should require the Supervisor to login via email and password. Then he will see a list of staff members currently assigned to him. The list is updated via a websocket, sending new or updating existing staff members. The Supervisor can tap on any staff member to see more details.

Write your code having in mind that you will hand it over to another developer who will take care of further support and feature implementation.

## 🚦 Before You Start

⚠️ Do not fork this repository.

Instead:

1. Create a new GitHub repository.
2. Start building your solution.
3. When you're done, push it to your GitHub and share the link or send a ZIP.

## 📋 Requirements

Your task is to create the Android App according to the principles of Clean Code with a distinct separation of the representation level from the repository level. The App shall not require a real API, so please mock any action that would normally require an API-Call.

### 🎨 UI Requirements

1. Create a LoginPage with email and passwort

   - Navigate to the StaffList upon successful registration

2. Create a StaffListPage

   - Create a ListItem showing
     - the full name of the Staff member
     - it's gender
     - it's photo
   - Create a List of ListItems and update it on incoming changes from the simulated Websocket

3. Create a StaffMemberPage
   - Upon tap on a ListItem navigate to a StaffMemberPage showing all details of the Staff member
   - show a placeholder instead of a photo if the staff member does not have a photo

### 🔌 Websocket Simulation

It is expected that you find a way to simulate incoming websocket data. This data can add, remove or update a Staff member to the existing list. It is expected that you find a solution that includes all 3 of the options:

- `add` a new staff member
- `remove` a staff member
- `update` a staff member

### 👤 StaffMember Entity:

A Staff member has the following properties:

- `firstName`
- `lastName`
- `age`
- `gender`
- `role` - Enum with values: security, catering, other
- `photo` (optional)

### 🖌️ UI Design

Feel free to use Material, Cuppertino or any other design library you prefer or create your own widgets.

### 🔄 State Management

You are free to choose any state management solution you prefer.

### 📦 External Packages

You are free to use any external package you think might be helpful.

### 🧪 Testing

Provide at least one unit test and one widget test.

## 🛠️ Extras (Optional)

You are free to implement none, one or multiple extras of the following list. It's optional, so you are welcome to stick to the ones you feel familiar with:

- Implement some basic validation with error information on the LoginPage
- Use only Custom Widgets. In case you want to use a Design Library, wrap the design library widget in a custom widget so that one could later change the design library without having to adjust the implementations of the widgets in the app
- Allow the supervisor to change a staff member's `role` and provide a confirmation flow. Update the list accordingly.
- Allow the supervisor to filter the staff list by its `role`
- Allow the Supervisor to delete a staff member from the list by swiping the list item
- Add some transition animation
- Use a router for the navigation
- Add a Splash Screen
- Add a Launcher Icon

## ✨ Vibe Coding

You are free to use AI Assistance for your coding. We assume that you do not implement any AI generated code that you are not able to explain or replicate yourself.

In case you do use AI Assistance, please save the chat history to a `CHAT_HISTORY.md` file and add it to your repository,

## 📤 Submission

Please submit your solution by providing:

- A GitHub repository link
- A `README.md` with setup instructions:
  - How to build and run the project locally

## ⏱️ Scope

This task is designed to take around 4 hours. Don't worry if you can't complete everything — that is not our primary interest.

Please focus on writing clean, well-structured code and demonstrating your thought process. There are thousand ways to Rome and we are neither interested in Rome itself nor if you got there - we are interested in the way that you choose.
