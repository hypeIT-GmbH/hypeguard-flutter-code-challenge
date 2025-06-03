# 📱 Flutter Challenge: Staff App

Welcome to the Flutter challenge! Please read the following carefully. In case any instructions are no clear, do not hesitate to contact us!. And please do not forget: This is a challenge, not a test. So enjoy!

## 📝 Scenario

Your goal is to build an Android App for an Event Supervisor, that allows the supervisor to see and edit the staff members that have been assigned to him. These staff members are subject to constant change during an event. The backend will inform the App via a Websocket on any changes related to the staff members. So the App must reflect those changes.

Th user should see a list of staff members currently assigned to him. The list is updated by incoming websocket data without any user interaction. The Supervisor can tap on any staff member to see more details.

Write your code having in mind that you will hand it over to another developer who will take care of further maintainance and feature implementation.

## 🚦 Before You Start

⚠️ Do not fork this repository.

Instead:

1. Create a new GitHub repository.
2. Start building your solution.
3. When you're done, push it to your GitHub and share the link or send a ZIP.

## 📋 Requirements

Your task is to create the Android App according to the principles of Clean Code with a distinct separation of the representation level from the repository level. The App shall not require a real API, so please mock any API calls or the websocket.

### 🎨 UI Requirements

1. Create a StaffListPage

   - Load the initial list of staff members from the repository
   - Create a ListItem showing
     - the full name of the Staff member
     - it's gender
     - it's photo
   - Create a List of ListItems and update it on incoming changes from the simulated Websocket

2. Create a StaffMemberPage
   - Upon tap on a ListItem navigate to a StaffMemberPage showing all details of the Staff member
   - show a placeholder instead of a photo if the staff member does not have a photo

### 🔌 Websocket and API Mocking

You should mock any API calls for login or retrieving data. Try to find a way to mock incoming data from a websocket and update the UI accordingly without any user interaction. The mocked data should implement all of the following options:

- `add` a new staff member
- `remove` a staff member
- `update` a staff member

It should be seen on the UI that a staff member get's added, removed and updated. So please build a logic, that will generate data according to this requirement.

In case you are having problems with this, just continue with the other requirements and do not get stuck on it.

### 👤 StaffMember Entity:

A Staff member has the following properties:

- `id`
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

## 🛠️ Extras (1)

Do you have any small idea on that we might have been missing in our requirements?
Something useful, nice, fancy, totally useless but funny...? Cool, then show us!

**NOTE:**

- DO NOT implement more than 1 Extra
- Do something that you are very familiar with
- Keep it simple (no more than 30 minutes on this!)

## ✨ Vibe Coding

You are free to use AI Assistance for your coding. We assume that you do not implement any AI generated code that you are not able to explain.

In case you do use AI Assistance, please save the chat history to a `CHAT_HISTORY.md`

## 📤 Submission

Please submit your solution by providing:

- An invitiation to your Github repository or sending us the zipped project
- A `README.md` with setup instructions:
  - How to build and run the project locally

## ⏱️ Scope

This task is designed to take a maximum of 4 hours. Don't worry if you can't complete everything — we really do not judge you by the amount of code you produce!

Please focus on writing clean, well-structured code and demonstrating your thought process.

There are thousand ways to Rome and we are neither interested in Rome itself nor if you got there - we are interested in the way that you choose.
