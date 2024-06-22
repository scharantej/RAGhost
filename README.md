## Flask Application Design for a RAG Web App

### HTML Files

- **index.html**: The main page of the application that will display the RAG status of tasks. This file will include HTML elements to render a table or list showcasing the tasks and their respective statuses (Red, Amber, Green).

### Routes

- **@app.route('/')**: This route will be associated with the index.html file and will serve as the homepage of the application. It will display the list of tasks and their RAG statuses.
- **@app.route('/add_task', methods=['POST'])**: This route will handle the addition of new tasks to the application. It will utilize the POST method to receive user input via a form and add the new task to a database or data structure.
- **@app.route('/update_task/<task_id>', methods=['POST'])**: This route will be used to update the status of an existing task. It will receive the task ID as a parameter and update the status based on user input.
- **@app.route('/delete_task/<task_id>', methods=['POST'])**: This route will handle the deletion of a task from the application. It will receive the task ID as a parameter and remove the task from the database or data structure.