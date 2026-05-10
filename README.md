# SignalR Samples

An **ASP.NET Core MVC application** showcasing multiple real-time communication patterns using **SignalR** — including group messaging, live order notifications, chat rooms, and user presence tracking.

## What it does

A collection of SignalR hub implementations demonstrating different real-time use cases — from simple broadcast messages to group-based and user-targeted communication.

## Tech Stack

- **ASP.NET Core MVC** (.NET)
- **SignalR** — real-time WebSocket communication
- **ASP.NET Identity** — user authentication
- **Entity Framework Core** — SQL Server

## SignalR Hubs

| Hub | Description |
|---|---|
| `ChatHub` | Real-time chat room messaging |
| `NotificationHub` | Broadcast notifications to all clients |
| `OrderHub` | Live order status updates |
| `PresenceHub` / `UserHub` | Track online/offline user presence |
| `HouseGroupHub` | Group-based messaging |
| `DeathlyHallowsHub` | Themed group communication example |

## Key Features

- Multiple hub types in one application
- Group membership management
- User-targeted messaging
- Connection lifecycle tracking (OnConnected / OnDisconnected)
- Identity integration for authenticated SignalR connections

## Getting Started

1. Set connection string in `appsettings.json`.
2. Apply migrations: `dotnet ef database update`
3. Run: `dotnet run --project SignalR_Samples`
