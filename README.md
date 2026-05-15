# Node.js-for-DevOps-Engineers

![NodeJS](https://img.shields.io/badge/node.js-6DA55F.svg?style=for-the-badge&logo=node.js&logoColor=white)

![](Nodejs.png)

## Node

<details>
<summary><b><i>1.What is Nodejs?</i></b></summary>

$\color{green}{\text{Answer}}$

Node.js is an open-source, cross-platform JavaScript runtime environment that allows developers to build server-side and networking applications.

</details>

<details>
<summary><b><i>2.How many threads does nodejs have?</i></b></summary>

$\color{green}{\text{Answer}}$

Nodejs is a single threaded langauage. It handles one operation at a time.

</details>

<details>
<summary><b><i>3.How do nodejs work?</i></b></summary>

$\color{green}{\text{Answer}}$

Node.js works by executing JavaScript code in a runtime environment outside of a web browser.

</details>

<details>
<summary><b><i>4.Is Nodejs Single Threaded Or Multi Threaded?</i></b></summary>

$\color{green}{\text{Answer}}$

Node.js is single-threaded for execution (to avoid complexity like race conditions) but multi-threaded for operations (to maintain high performance).

</details>

<details>
<summary><b><i>5.What is node cluster?</i></b></summary>

$\color{green}{\text{Answer}}$

A Node.js cluster is a module that allows you to run multiple instances of your application (called workers) to handle incoming traffic, effectively utilizing all available CPU cores.

</details>

<details>
<summary><b><i>6.Does parent process depends on the child preocess?</i></b></summary>

$\color{green}{\text{Answer}}$

No, the Parent process does not depend on Child processes for its own execution.

</details>

<details>
<summary><b><i>7.How many types of module do nodejs have?</i></b></summary>

$\color{green}{\text{Answer}}$

Node.js has three main types of modules:
- Core Modules: Built-in modules that come with the Node.js installation (e.g., `fs`, `http`, `path`, `os`).

- Local Modules: Files created by you within your application (e.g., `./myLogger.js`).

- Third-Party Modules: Packages installed via NPM or Yarn (e.g., `express`, `mongoose`, `dotenv`).

</details>

<details>
<summary><b><i>8.Why nodejs?</i></b></summary>

$\color{green}{\text{Answer}}$

Node.js is chosen for its efficiency in building scalable, real-time applications.

- Speed: Powered by Google’s V8 engine, it compiles JavaScript directly to machine code.

- Non-blocking I/O: Handles thousands of concurrent connections without waiting for tasks (like database queries) to finish.

- Unified Language: Uses JavaScript for both frontend and backend, simplifying development.

- Massive Ecosystem: Access to over 2 million packages via NPM to accelerate building.

- Lightweight: Excellent for microservices and containerized environments (like Docker).

</details>

<details>
<summary><b><i>9.What is npm?</i></b></summary>

$\color{green}{\text{Answer}}$

npm (Node Package Manager) is the default package manager for Node.js. It consists of two main parts:

- The Registry: A massive online database of public and private JavaScript packages.

- The CLI: A command-line tool used to install, update, and manage those packages in your projects.

</details>

<details>
<summary><b><i>10.Difference between pacakage.json and pacakage-lock.json?</i></b></summary>

$\color{green}{\text{Answer}}$

They work together to manage your project's dependencies:

- `package.json`: Acts as a manifest. It lists the packages your project needs and uses semantic versioning ranges (e.g., `^1.2.0`). This allows for minor updates when someone else runs npm install.

- `package-lock.json`: Acts as a snapshot. It records the exact version of every package and its sub-dependencies currently installed. This ensures that every developer and environment (like a production server) uses the identical dependency tree.

</details>

<details>
<summary><b><i>11.What is the difference betwwen creating a server with http and a framework?</i></b></summary>

$\color{green}{\text{Answer}}$

The main difference is abstraction and speed of development.

1. Using the http Core Module
   - This is a "low-level" approach. You are using Node's built-in tools without any external help.

   - Manual Labor: You must manually parse URLs, handle HTTP methods (GET vs. POST), and set headers/status codes.

   - Boilerplate: Even simple tasks like serving an image or parsing JSON require many lines of code.

   - Performance: Slightly faster because there is no overhead, but the difference is negligible for most apps.

2. Using a Framework (e.g., Express, Fastify)
   - This is a "high-level" approach built on top of the http module.

   - Routing: Simple, readable syntax for defining endpoints (e.g., app.get('/users')).

   - Middleware: Easy integration for tasks like logging, security, and body parsing.

   - Standardization: Provides a structured way to organize your code, making it easier for teams to collaborate.

</details>

<details>
<summary><b><i>12.What do you mean by non-blocking?</i></b></summary>

$\color{green}{\text{Answer}}$

Non-blocking means Node.js can start a task (like reading a file or querying a database) and immediately move to the next line of code without waiting for that task to finish.

</details>

<details>
<summary><b><i>13.What is event loop?</i></b></summary>

$\color{green}{\text{Answer}}$

The Event Loop is the mechanism that allows Node.js to perform non-blocking I/O operations despite being single-threaded. It offloads tasks to the system kernel whenever possible.

</details>

<details>
<summary><b><i>14.What is event driven?</i></b></summary>

$\color{green}{\text{Answer}}$

Event-driven is a programming paradigm where the flow of the program is determined by events—such as user actions (clicks), sensor outputs, or messages from other programs.

In Node.js, this is implemented through the EventEmitter class and the Event Loop.

- Event Emitter: The object that sends a signal that something has happened.

- Event Handler: The function that contains the logic to be executed when the signal is received.

</details>
