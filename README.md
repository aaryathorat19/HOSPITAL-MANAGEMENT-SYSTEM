# HOSPITAL-MANAGEMENT-SYSTEM
# Description of the Hospital Management System Code
This C program provides a simple Hospital Management System that manages patients and their appointments using Data Structures and Algorithms (DSA), specifically Linked Lists and Queues. Here's a detailed description of how the system works:

# Key Data Structures Used:
1. Linked List:

A linked list is used to manage the patients in the system. Each node in the linked list represents a patient with details such as Patient ID, Name, and Ailment.
The linked list allows dynamic addition and deletion of patients.
2. Queue:

A queue is used to manage appointments in the system. The queue follows a First-Come-First-Served (FCFS) approach, where the first appointment scheduled will be the first one to be processed.
The queue has two pointers:
front: Points to the first appointment in the queue.
rear: Points to the last appointment in the queue.

# Key Functionalities:
1. Add Patient:

This option allows the user to add a new patient to the system by providing their details: Patient ID, Name, and Ailment.
The patient is added to the linked list at the end.
2. Search Patient:

The system allows searching for a patient by their name.
It traverses the linked list and returns the patient's details if a match is found.
3. Delete Patient:

This option removes a patient from the system based on their Patient ID.
The system traverses the linked list, finds the patient with the matching ID, and deletes that patient.
4. Display Patients:

Displays the details of all patients registered in the system by traversing the linked list from the beginning to the end.
5. Schedule Appointment:

This option allows the user to schedule an appointment for a registered patient.
If the patient is found in the system, their appointment is added to the queue. If the patient is not found, the system prompts the user to register the patient first.
6. Process Appointment:

Processes the next appointment from the queue in First-Come-First-Served (FCFS) order.
The first patient in the queue is processed, and their appointment is removed from the queue.
# Detailed Explanation of Key Functions:
1.) Patient Management (Linked List):

A. createPatient:
Allocates memory for a new patient node and initializes it with the patient's details (id, name, ailment).
B. addPatient:
This function inserts a new patient at the end of the linked list. If the list is empty, the new patient becomes the first node.
C. searchPatient:
This function searches for a patient by their name. It traverses the linked list and returns a pointer to the patient node if found, or NULL if not found.
D. deletePatient:
Deletes a patient from the linked list based on their Patient ID. The function handles cases where the patient to be deleted is either the head, a middle node, or the last node.
E. displayPatients:
This function traverses the linked list and prints the details of each patient.
2.) Appointment Management (Queue):

A. createQueue:
Initializes an empty queue with front and rear pointers set to NULL.
enqueue:
Adds a new appointment to the rear of the queue. If the queue is empty, the new appointment becomes both the front and rear. Otherwise, it is added to the end of the queue.
dequeue:
Removes the appointment at the front of the queue (i.e., the first scheduled appointment) and processes it. If the queue is empty, a message indicating that no appointments are available is displayed.
Working of the System (User Flow):
Adding a Patient:

The user is prompted to enter a patient's ID, Name, and Ailment.
The system creates a new patient node and adds it to the linked list.
3.) Searching for a Patient:

The user can search for a patient by entering their name. If the patient is found in the linked list, the system displays their details.
4.) Deleting a Patient:

The user can delete a patient by entering their ID. The system searches the linked list for the patient with the matching ID and removes them.
5.) Displaying All Patients:

The system lists all registered patients by traversing the linked list.
6.) Scheduling an Appointment:

The user can schedule an appointment for a registered patient by entering their Patient ID.
If the patient is found, their appointment is added to the queue.
7.) Processing Appointments:

The system processes appointments in the order they were scheduled. The first appointment in the queue is processed and removed.
## Use of DSA (Data Structures and Algorithms):
# Linked List:

The system uses a singly linked list to manage patient records. Linked lists allow dynamic memory allocation, making it easy to add or delete patients without worrying about fixed memory blocks.
# Queue:

A queue is used to manage patient appointments in First-Come-First-Served (FCFS) order. The enqueue operation adds a patient’s appointment to the end of the queue, and dequeue processes the appointment at the front of the queue.

## Future Enhancements:
File handling: Save patient records and appointments to a file for persistence across sessions.
Priority queue: Manage appointments based on the severity of ailments using a priority queue.
Editing patient details: Add functionality to update or edit patient information.
This simple Hospital Management System demonstrates the use of basic DSA concepts in building a functional system for managing patients and appointments.
