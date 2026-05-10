# SignalR Samples

An **ASP.NET Core MVC application** showcasing multiple real-time communication patterns using **SignalR** — including group messaging, live order notifications, chat rooms, and user presence tracking.

## What it does

This project is a collection of SignalR hub implementations demonstrating different real-time use cases. Each hub illustrates a specific pattern — from simple broadcast messages to group-based and user-targeted communication.

## Tech Stack

- **ASP.NET Core MVC** (.NET)
- **SignalR** — real-time WebSocket communication
- **ASP.NET Identity** — user authentication
- **Entity Framework Core** — SQL Server

## SignalR Hubs

| Hub | Description |
|---|---|
| `ChatHub` | Real-time chat room messaging |
| `NotificationHub` | Broadcast notifications to all connected clients |
| `OrderHub` | Live order status updates |
| `PresenceHub` / `UserHub` | Track online/offline user presence |
| `HouseGroupHub` | Group-based messaging (send to specific groups) |
| `DeathlyHallowsHub` | Themed group communication example |

## Key Features

- Multiple hub types in a single application
- Group membership management
- User-targeted messaging
- Connection lifecycle tracking (OnConnected / OnDisconnected)
- Identity integration for authenticated SignalR connections

## Getting Started

1. Set your SQL Server connection string in `appsettings.json`.
2. Apply migrations:
   ```bash
   dotnet ef database update
   ```
3. Run the app:
   ```bash
   dotnet run --project SignalR_Samples
   ```
