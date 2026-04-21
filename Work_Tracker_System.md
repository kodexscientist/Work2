# Work Tracker System

## Overview
This document outlines a comprehensive work tracker system for policy professionals. The system includes databases for tasks, subtasks, dependencies, and contacts, along with project management views, completion tracking, due dates, resource management, and point of contact tracking.

---

## 1. Databases
### 1.1 Tasks Database
- **Task ID**: Unique identifier for each task.
- **Task Name**: Descriptive name of the task.
- **Due Date**: Deadline for task completion.
- **Priority**: Assigned priority level (High, Medium, Low).
- **Status**: Current status (Not Started, In Progress, Completed, Blocked).
- **Assignee**: Person responsible for the task.

### 1.2 Subtasks Database
- **Subtask ID**: Unique identifier for each subtask.
- **Parent Task ID**: ID of the parent task.
- **Subtask Name**: Descriptive name of the subtask.
- **Due Date**: Deadline for subtask completion.
- **Status**: Current status.

### 1.3 Dependencies Database
- **Dependency ID**: Unique identifier for each dependency.
- **Task ID**: ID of the task that has dependencies.
- **Dependent Task ID**: ID of the task that is dependent on the above task.

### 1.4 Contacts Database
- **Contact ID**: Unique identifier for each contact.
- **Name**: Full name of the contact.
- **Role**: Role in the project (e.g., Stakeholder, Team Member).
- **Email**: Contact email address.
- **Phone**: Contact phone number.

---

## 2. Project Management Views
### 2.1 Kanban Board
- Visual representation of tasks and subtasks in columns representing different statuses.
### 2.2 Gantt Chart
- Timeline view to show task durations and dependencies visually.

---

## 3. Completion Tracking
- Track percentage of task/subtask completion.
- Visual indicators (like progress bars) for each task.

---

## 4. Due Dates
- A calendar integration to manage and visualize due dates for tasks.

---

## 5. Resource Management
- Allocation of resources per task.
- Tracking availability and workload of team members.

---

## 6. Point of Contact Tracking
- Maintain a list of points of contact for each major task.
- Quick access to contact information directly from the task view.

---

## Conclusion
This work tracker system is designed to enhance the efficiency and effectiveness of project management for policy professionals, enabling them to manage their tasks comprehensively and collaboratively.