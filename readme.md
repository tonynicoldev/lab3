# Price List front and back integration
This demo follows up on the previous frontend and backend demos. When you understand this, you will be more than ready to integrate your joke front and backends.

## Debugging
To debug the frontend and the backend at the same time, you could run the backend in the vscode debugger and use the browser debugger. Alternatively, you can configure VScode to run multiple debug sessions by writing a launch.json config file. I've provided one for you and it needs to be called launch.json and needs to live in a dir called .vscode

If you keep the same app name and port number you won't need to edit the file for your lab exercise but the file is pretty readable so easy to modify if needed.

To launch the debug session, don't use F5. Click on the debug icon in the left hand menu then in the Run and Debug dropdown, select backend, frontend or full stack to debug both.

You can only debug JavaScript, but you can set breakpoints on the frontend and backend JavaScript making this incredibly helpful for debugging.

## New Stuff
I've added a couple of new techniques. Loading the data using a file as opposed to using require. You can use require if you want so you have less code to change, but here I use a file for demo purposes.

I use path.join to show you how you can build up a file path using this function. This can be useful when moving to a different operating system as filepaths can become tricky if you define them as a fixed string. We will soon be using Linux.

I've used a static web server to deploy the web assets from a dir called public.

I've added express.json() as I'm POSTing to the backend and providing body data in json format so I need this function to parse the json into the request object.

The main addition to your current code is probably the use of async / await and fetch to make the API calls.

This demo covers everything you need to know to implement the lab exercise.


