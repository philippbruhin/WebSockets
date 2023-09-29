# WebSockets

Building a websocket server, based on [this](https://youtu.be/2Nt-ZrNP22A?si=O1e7JSUyiWchj066) YoutTube tutorial.

The repo is using Node in Version `v18.12.1`.

1. Clone this repo with `git clone git@github.com:philippbruhin/WebSockets.git`.
2. Cd into the project and run `npm install`.
3. In VSCode click **Run > Start Debugging** and open the Debug Console.
4. Open Google Chrome developer tools and add following commands in the console:

    ```
    let ws = new WebSocket("ws://localhost:8080");
    ws.onmessage = message => console.log(`Received: ${message.data}`);
    ws.send("Hello! I'm client.")
    ```
