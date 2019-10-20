<h1 align="center">
    <img alt="GoStack" src=".github/logo.png" width="200px" />
</h1>

<h3 align="center">
 Challenge 1: NodeJS Concepts
</h3>

### About the challenge 1
Application to store projects and their tasks from scratch using Express.

### Rotas
- `POST / projects`: The route should get` id` and `title` inside the body and register a new project into an array in the following format:` {id: "1", title: 'New project', tasks : []} `; Be sure to submit both the project ID and title in double-quoted string format.

- `GET / projects`: Route that lists all projects and their tasks;

- `PUT / projects /: id`: The route should only change the project title with the` id` present in the route parameters;

- `DELETE / projects /: id`: The route must delete the project with the` id` present in the route parameters;

- `POST / projects /: id / tasks`: The route must receive a` title` field and store a new task in the task array of a specific project chosen through the `id` present in the route parameters.

### Middlewares
- Create middleware that will be used on all routes that receive the project ID in the URL parameters that check if the project with that ID exists. If none exists return an error, otherwise allow the request to continue normally;

Create a global middleware called on all requests that prints (`console.log`) a count of how many requests have been made in the application so far.
