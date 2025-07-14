

- GameKit
-  GKMatchmakerViewControllerDelegate 

Protocol

# GKMatchmakerViewControllerDelegate

An object that handles when the status of matchmaking changes.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
protocol GKMatchmakerViewControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Finding multiple players for a game

## Overview

The delegate of a GKMatchmakerViewController object implements this protocol to handle when players accept invitations, the player cancels matchmaking, or an error occurs. In all these cases, except when a hosted player accepts a invitation, for example, matchmakerViewController(_:hostedPlayerDidAccept:), the delegate needs to dismiss the view controller.

## Topics

### Starting matches

func matchmakerViewController(GKMatchmakerViewController, didFind: GKMatch)

Handles when the view controller finds players for a peer-to-peer match.

func matchmakerViewController(GKMatchmakerViewController, didFindHostedPlayers: [GKPlayer])

Handles when the view controller finds all requested players for a hosted match.

### Matching players using rules

func matchmakerViewController(GKMatchmakerViewController, getMatchPropertiesForRecipient: GKPlayer, withCompletionHandler: ([String : Any]) -> Void)

Returns the properties for another player that the local player invites using the view controller interface.

### Handling cancellations and errors

func matchmakerViewControllerWasCancelled(GKMatchmakerViewController)

Handles when a player cancels a request to find players for a match.

**Required**

func matchmakerViewController(GKMatchmakerViewController, didFailWithError: any Error)

Handles when a view controller encounters an error while finding players for a match.

**Required**

### Hosting matches

func matchmakerViewController(GKMatchmakerViewController, hostedPlayerDidAccept: GKPlayer)

Handles when a player in a hosted match accepts the invitation.

### Deprecated Methods

func matchmakerViewController(GKMatchmakerViewController, didFindPlayers: [String])

Called when a hosted match is found.

Deprecated

func matchmakerViewController(GKMatchmakerViewController, didReceiveAcceptFromHostedPlayer: String)

Called when a player in a hosted match accepts the invitation.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the delegate

var matchmakerDelegate: (any GKMatchmakerViewControllerDelegate)?

The object that handles matchmaker view controller changes.

