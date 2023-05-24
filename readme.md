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

---
## Links:
* [Tutorial: Get started with ASP.NET Core SignalR](https://learn.microsoft.com/en-us/aspnet/core/tutorials/signalr?view=aspnetcore-7.0&tabs=visual-studio)
* [Introduction to SignalR](https://learn.microsoft.com/en-us/aspnet/signalr/overview/getting-started/introduction-to-signalr)
* [SignalR on Github](https://github.com/signalr)