# TaskFlow API Reference

## Overview
The TaskFlow API allows clients to create, retrieve, and delete tasks.

## Base URL
https://api.taskflow.example.com

## GET /tasks

Description
Retrieve all tasks.

Request
GET /tasks

Response
[
  {
    "id": 101,
    "name": "Prepare sprint report",
    "status": "in_progress"
  }
]

---

## POST /tasks

Description
Create a new task.

Request
POST /tasks

Body
{
  "name": "Draft release notes",
  "status": "open"
}

Response
{
  "id": 103,
  "name": "Draft release notes",
  "status": "open"
}

---

## DELETE /tasks/{id}

Description
Delete a task.

Request
DELETE /tasks/103

Response
{
  "message": "Task deleted successfully"
}
