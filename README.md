# Software Project I - Practice Assignment 1

## Task: Filter & Search Todos

I completed the Todo filtering task using server-side filtering.

## Backend

Updated `todoController.js` to support filtering todos using the `done` query parameter.

### Supported Requests

- `GET /api/todos` - Returns all todos.
- `GET /api/todos?done=true` - Returns completed todos.
- `GET /api/todos?done=false` - Returns incomplete todos.

The `done` parameter is read from `req.query` and passed as a filter to `Todo.find()`.

## Frontend

Updated the frontend to support filtering through three options:

- **All** - Shows all todos.
- **Active** - Shows incomplete todos.
- **Done** - Shows completed todos.

The selected filter is stored in React state, and the todos are fetched again whenever the filter changes.

The frontend sends the appropriate query parameter to the backend.

## Completed

- Backend todo filtering
- Frontend filter state
- All / Active / Done buttons
- Server-side filtering with query parameters
- Frontend re-fetching when the filter changes
