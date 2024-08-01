# Task Management API Documentation
the link for the postman api documentation is
https://documenter.getpostman.com/view/37345989/2sA3kdAxc5

over view  

## Endpoints

### GET /tasks
- Description: Get a list of all tasks.
- Response:
  - Status: 200 OK
  - Body: Array of tasks

### GET /tasks/:id
- Description: Get the details of a specific task.
- Parameters:
  - id: Task ID
- Response:
  - Status: 200 OK
  - Body: Task object
  - Status: 404 Not Found (if task not found)

### POST /tasks
- Description: Create a new task.
- Request:
  - Body: Task object (title, description, due date, status)
- Response:
  - Status: 201 Created
  - Body: Created task object

### PUT /tasks/:id
- Description: Update a specific task.
- Parameters:
  - id: Task ID
- Request:
  - Body: Task object (title, description, due date, status)
- Response:
  - Status: 200 OK
  - Body: Updated task object
  - Status: 404 Not Found (if task not found)

### DELETE /tasks/:id
- Description: Delete a specific task.
- Parameters:
  - id: Task ID
- Response:
  - Status: 204 No Content
  - Status: 404 Not Found (if task not found)


