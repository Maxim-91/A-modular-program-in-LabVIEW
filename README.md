# Modular Program in LabVIEW

This LabVIEW project demonstrates the use of modular architecture, user events, and dynamic VI execution to manage tasks efficiently. The project highlights the separation of tasks into independent subVIs that communicate via user events, providing a structured and scalable solution.

## Key Features

1. **Modular Architecture**:
   - The program follows a modular design where each task is managed by an independent subVI.
   - The main VI controls the overall process flow, dynamically launching subVIs as needed.

2. **User Event Communication**:
   - The program uses user events to pass control signals and data between the main VI and subVIs.
   - Events such as starting number generation or stopping a process are triggered and handled efficiently.

3. **Dynamic Execution of SubVIs**:
   - SubVIs are launched dynamically during runtime based on user input or predefined events.
   - This allows for parallel execution of tasks and modular control of different processes.

4. **Event-Driven Process Control**:
   - Processes such as number generation are initiated based on user event triggers.
   - The program listens for specific events and performs actions, such as starting a generator or displaying results, based on the event type.

5. **Result Display**:
   - Results from the number generation process are passed back to the main VI and displayed in real-time.
   - The user can observe the output dynamically, enhancing interactivity and user control.

## Program Workflow

1. **Main VI Initialization**:
   - The main VI initializes user events and prepares for dynamic subVI execution.
   - User events such as "Generate Numbers" or "Stop" are registered and ready to be handled.

2. **User-Triggered Events**:
   - The program listens for specific events triggered by user actions (e.g., "Start Generating Numbers").
   - Once triggered, the corresponding subVI is dynamically launched to handle the task.

3. **SubVI Execution**:
   - The subVI (`Gener.vi`) handles the number generation process once the event is triggered.
   - The subVI runs independently and returns the result to the main VI for display.

4. **Termination and Event Handling**:
   - User can trigger events to stop or exit the process at any time.
   - The main VI listens for these termination events and safely stops the subVIs without interrupting other tasks.

## Inputs and Outputs

- **Inputs**:
  - User events that initiate actions like generating numbers or stopping processes.

- **Outputs**:
  - The result from the subVI is displayed in the main VI in real-time.

## How to Use

1. Launch the main program in LabVIEW.
2. Trigger events such as starting the number generator via the user interface.
3. Observe the generated results displayed dynamically in the main VI.
4. Safely stop or exit the program using the provided controls.

## Requirements

- **LabVIEW** version XX.X or later.
- Familiarity with event-based programming and modular architecture in LabVIEW.

## Notes

- This project showcases the power of dynamic VI execution and user event handling.
- It provides a flexible and scalable way to manage multiple processes asynchronously.

## Code
![image](https://github.com/user-attachments/assets/a1510f7b-4fe3-45af-96a0-e1627889d425)
![image](https://github.com/user-attachments/assets/18b3e920-a800-43f8-8db2-08a86c9fc8c4)
![image](https://github.com/user-attachments/assets/4ab85652-1bc4-432d-b29a-1e48880a3db0)
![image](https://github.com/user-attachments/assets/418207f2-74c8-4ab7-85e4-9a25341eda68)

## The appearance of the running program
![image](https://github.com/user-attachments/assets/48d4b033-4db6-41f2-92c6-a55648294004)
![image](https://github.com/user-attachments/assets/433e0841-b7e3-41da-90b2-6aa876f40496)
