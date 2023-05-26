# Demo SignalR with ASP.NET Core

## What is SignalR?
>ASP.NET SignalR is a library for ASP.NET developers that simplifies the process of adding real-time web functionality to applications.

>SignalR provides a simple API for creating server-to-client remote procedure calls (RPC) that call JavaScript functions in client browsers (and other client platforms) from server-side .NET code. SignalR also includes API for connection management (for instance, connect and disconnect events), and grouping connections.

>SignalR applications can scale out to thousands of clients using built-in, and third-party scale-out providers.

## Built-in providers include:
* Service Bus
* SQL Server
* Redis

## Third-party providers include:
* NCache

## SignalR and WebSocket
>SignalR uses the new WebSocket transport where available and falls back to older transports where necessary.

## Transports and fallbacks
* WebSocket (the optimal transport for SignalR)
* Server Sent Events (aka EventSource )
* Forever Frame (for Internet Explorer only)
* Ajax long polling

## Monitoring transports
You can determine what transport your application is using by enabling logging on your hub, and opening the console window in your browser. To enable logging for your hub's events in a browser, add the following command to your client application:

`$.connection.hub.logging = true;`

## Connections and Hubs
The SignalR API contains two models for communicating between clients and servers: 
1. **Persistent Connections**. A Connection represents a simple endpoint for sending single-recipient, grouped, or broadcast messages.
2. **Hubs**. A Hub is a more high-level pipeline built upon the Connection API that allows your client and server to call methods on each other directly.

## How Hubs work
>When server-side code calls a method on the client, a packet is sent across the active transport that contains the name and parameters of the method to be called (when an object is sent as a method parameter, it is serialized using JSON). The client then matches the method name to methods defined in client-side code. If there is a match, the client method will be executed using the deserialized parameter data.

---
## Links:
* [Tutorial: Get started with ASP.NET Core SignalR](https://learn.microsoft.com/en-us/aspnet/core/tutorials/signalr?view=aspnetcore-7.0&tabs=visual-studio)
* [Introduction to SignalR](https://learn.microsoft.com/en-us/aspnet/signalr/overview/getting-started/introduction-to-signalr)
* [SignalR on Github](https://github.com/signalr)