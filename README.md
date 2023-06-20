# Postman Collection for API Testing

This repository contains a Postman collection for testing various endpoints of the JSON Placeholder API. The tests include:

1. Get all posts and verify the status code;
2. Create a new post and verify the response;
3. Update an existing post and verify the update;
4. Delete an existing post and verify the deletion.

## API Description

We're using the JSON Placeholder API ([https://jsonplaceholder.typicode.com/](https://jsonplaceholder.typicode.com)) for our tests. This is a simple, free REST API that provides placeholder data for testing and prototyping. The endpoints that we're testing involve the `/posts` resource, which simulates a blog post system.

## Tests Description

1. `GET /posts` - retrieves a list of all posts. The test verifies that the status code is 200.
2. `POST /posts` - creates a new post. The test verifies that the response has correst status code, and has a response body and includes the ID of the new post, which we set to environments variables.
3. `PUT /posts/:id` - updates an existing post. The test verifies that the returned post includes the updated information.
4. `DELETE /posts/:id` - deletes an existing post. The test verifies that the response status is 200, indicating a successful deletion.

## How to Import and Run the Postman Collection

1. Download the collection JSON file from this repository.
2. Open Postman.
3. Click on the "Import" button on the top left.
4. Choose the downloaded JSON file to import.
5. Once imported, the collection will appear in the left sidebar under "Collections".
6. Select Environments in the sidebar and select jsonplaceholder, after that set "current value" for jsonplaceholder_prod to be the same as "initial value".
7. Set "current value" for "userId" in the Collections variables to be the same as "initial value".
8. To run the tests, click on the arrow next to the collection name and then click "Run".
9. A new window will appear. Click "Run" again to start the tests.

## Screenshots of Test Results

1. A screenshot of the result of the "Get all posts" test:
![Get all posts](https://i.ibb.co/QcrdK2w/Screenshot-2023-06-20-at-16-09-37.png)

2. A screenshot of the result of the "Create a new post" test:
![Create a new post](https://i.ibb.co/r7g8GL0/Screenshot-2023-06-20-at-16-09-57.png)

3. A screenshot of the result of the "Update a post" test.
![Update a post](https://i.ibb.co/z7m7TD8/Screenshot-2023-06-20-at-16-10-12.png)

4. A screenshot of the result of the "Delete a post" test.
![Delete a post](https://i.ibb.co/9ck2NkY/Screenshot-2023-06-20-at-16-10-29.png)
