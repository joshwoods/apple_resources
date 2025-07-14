

- GameKit
- GKGameSessionSharingViewController
-  init(session:) Deprecated

Initializer

# init(session:)

Creates a new sharing view controller for a specified session.

tvOS 10.0–12.0Deprecated

``` source
@MainActor
init(session: GKGameSession)
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

