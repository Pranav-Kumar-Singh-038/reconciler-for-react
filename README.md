# Todo List Reconciler for React

This project demonstrates a simplified version of a reconciler mechanism inspired by React, implemented in vanilla JavaScript. It provides a dynamic way to manage a todo list, supporting operations such as adding todos, marking them as done, and automatically updating the DOM to reflect changes in the todo list state.

## Features

- **Add Todos**: Users can add todos with a title and description.
- **Mark as Done**: Todos can be marked as done and are removed from the list.
- **State Reconciliation**: The mechanism compares the new state with the old one to determine which todos have been added, updated, or removed, and makes the necessary DOM updates efficiently.

## Usage

1. **Adding a Todo**: Enter the title and description of the todo in the respective input fields and click the "Add todo" button. The todo will appear below.
2. **Marking a Todo as Done**: Each todo item has a "Mark as Done" button. Clicking this button will remove the todo from the list.
3. **Changing State**: The "Change" button simulates an external update to the todo list state, showcasing the reconciler's ability to update the DOM based on state changes.

## How It Works

- The application maintains a todo state in memory, which is an array of todo objects.
- Each todo object contains a title, description, and a unique ID.
- When the state changes, the reconciler (`updateState` function) compares the new state with the old one to determine which todos have been added, removed, or updated.
- Based on this comparison, the reconciler makes the minimal set of DOM updates required to reflect the state change.
