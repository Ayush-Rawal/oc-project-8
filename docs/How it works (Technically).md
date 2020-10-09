# How it works (Technically)

## The MVC Architecture
The Model-View-Controller architecture is a common software design architecture that divides a software into three layers to enforce seperation of concerns. It is easier to develop, maintain, and test these loosely coupled individual layers.

### The Model layer
The model layer is responsible for handling data. This includes representing data within the app, persisting data across different kinds of storage, and translating data across models

### The View layer
The view layer is responsible for displaying the user interface

### The Controller layer
The controller layer is responsible for handling user input and interactions

## Project Structure
The project is built on MVC architecture.

### Model
The store.js and model.js files contain the model layer. The Model class provides CRUD and getCount operations for todos relying on the Store class to manage data storage. The store class uses the browsers local storage to store app data relying on an in-memory object data store as a backup incase local storage is not available.

### View
The view.js and template.js files contain the view layer. The template file contains html string templates for different ui elements that have placeholders for data. They take in data from the model layer, replace the placeholder with them and return the ui html.

### Controller
The controller.js file contains the controller layer. It is responsible for handling user interaction. It queries and updates the models and trigger view renders in response to user actions.

### Tests
The project uses the jasmine library to run automated tests. These help in making sure the software works as expected after making changes. 
