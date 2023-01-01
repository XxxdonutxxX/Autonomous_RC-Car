# Autonomous RC-Car

## Description
This project uses the same idea as NASA's rovers going on missions to explore surfeces like Mars, Moon, and astroids. Rovers on other surfaces don't have GPS and navigation systems like we do here on Earth. So they use sensors and mapping softwares so the rover knows where to go and what to avoid in real-time.

This project uses the same idea as NASA's rovers, where it goes around the place, mapping everything around it. The difference is, it needs to know when the object is stationary object or moving object. If it's a stionary object, it will store this data inside a file so that next time when the car goes to this place, it would know that there is an object in that area, so avoid it. In other words, if it was in a room, it will map stuff like bed, table, walls, etc. However, if the object is moving, like a human or a pet, it would check every once in a while to see if the path that moving object was at moved or not. If it moved, then the car can go in that path.

This project uses Swift for the GUI and communication between the Raspberry Pi and the computer hosting the server, C++ with Arduino framework to move the car, Python for image recognition.

Currently, this application will only run on Mac because of Swift


## How to Install and Run the Project
TBA


## How to Use the Project
TBA


## Currently in the Work
  - Settings up the sockets and GUI
    - Use Swift GUI for Mac and use sockets to establish connection between the server on the machine and the Raspberry Pi.
  - Setting up image recognition
    - Set up a machine learning algorithm that knows stationry objects. And if there is an object that it can't identify, goes to next step.
    - If it reaches this step, it means it couldn't identify they object. So it watches it for 2 seconds. If no movements detected after that, it registers it as stationary object. In either way, it takes a screenshot of the object and stores it in a folder called "unidetefied objects". These objects will be then labeled as stationary or moving object for the machine learning to detect them. 
