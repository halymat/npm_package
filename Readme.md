1. ### What is the Event loop ?

   Event loop is an infinite loop and in each iteration it checks the event queue for any triggered event, if found it then executes it and removes it from the queue.

2. ### Explain the 6 phases of the event loop ?

   1. Timers Phase: This is the first phase in the event loop,In this phase, the event loop checks for any scheduled setTimeout() or setInterval() callbacks that have expired, and executes their callback functions.
   1. Pending callbacks phase: It handles I/O callbacks deferred to the next iteration, from the previous iteration of the event loop.
   1. Idle, prepare phase: It is an internal phase that is used to prepare for the upcoming poll phase.
   1. Poll phase: The Poll phase calculates the blocking time in every iteration to handle I/O callbacks
   1. Check phase: This phase handles the callbacks scheduled by setImmediate(), and the callbacks will be executed once the Poll phase becomes idle.
   1. Close phase: In this final phase,any close events that were triggered are handled,such as when a socket is closed.

3. ### List some best practices in server-side code development?

   1. Focus on Code Quality
   2. Prefer ES6+ and Async/Await
   3. Keep Code Small
   4. Handle Errors

4. ### What is NPM5: How do you initialize a package in npm?

   NPM stands for Node Package Manager. It is a command line tool that comes bundled with node.js, and it is used to manage packages libaries, frameworks and other code modules for node.js projects. To initialize a package in npm, npm init command.

5. ### How do you run a script in the package.json ?
   To run a script that you have added to your package.json file, simply run $ npm run argument with the name of the script as the argument.For example,
   npm run prettier
