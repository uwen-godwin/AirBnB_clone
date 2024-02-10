# AirBnB Clone

Welcome to the AirBnB clone project!

Before starting, please read the AirBnB concept page.

## Description

The AirBnB clone project aims to build a command-line interface (CLI) for managing AirBnB-like objects. This project serves as the first step towards building a full web application, providing the foundation for HTML/CSS templating, database storage, API, and front-end integration.
Each task is linked and will help you to:

- put in place a parent class (called BaseModel) to take care of the initialization, serialization and deserialization of your future instances
- create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file
- create all classes used for AirBnB (User, State, City, Place…) that inherit from BaseModel
- create the first abstracted storage engine of the project: File storage.
- create all unittests to validate all our classes and storage engine

## Command Interpreter
Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to be able to manage the objects of our project:

- Create a new object (ex: a new User or a new Place)
- Retrieve an object from a file, a database etc…
- Do operations on objects (count, compute stats, etc…)
- Update attributes of an object
- Destroy an object

### Description

The command interpreter is a crucial component of the AirBnB clone project. It allows users to manage objects by performing operations such as creating, retrieving, updating, and deleting instances of various classes.

### Execution

#### Interactive Mode

	Your shell should work like this in interactive mode:

	```bash
	$ ./console.py
	(hbnb) help

	Documented commands (type help <topic>):
	========================================
	EOF  help  quit

	(hbnb) 
	(hbnb) 
	(hbnb) quit
	$


#### Non-Interactive Mode
Your shell should also support non-interactive mode, similar to the Shell project in C:

	$ echo "help" | ./console.py
	(hbnb)

	Documented commands (type help <topic>):
	========================================
	EOF  help  quit
	(hbnb) 
	$

#### Running Tests
All tests should pass in non-interactive mode:

	$ echo "python3 -m unittest discover tests" | bash
