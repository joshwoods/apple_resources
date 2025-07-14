

- GameKit
-  GKTurnBasedMatchmakerViewControllerDelegate 

Protocol

# GKTurnBasedMatchmakerViewControllerDelegate

A protocol that handles when the status of turn-based matchmaking changes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
protocol GKTurnBasedMatchmakerViewControllerDelegate : NSObjectProtocol
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Overview

To receive notifications when a player cancels turn-based matchmaking or an error occurs, implement this protocol in the GKTurnBasedMatchmakerViewController object’s delegate.

## Topics

### Handling Cancellation and Errors

func turnBasedMatchmakerViewControllerWasCancelled(GKTurnBasedMatchmakerViewController)

Handles when the player dismisses the view controller without inviting players.

**Required**

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, didFailWithError: any Error)

Handles when an error occurs while the local player invites other players.

**Required**

### Deprecated Methods

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, didFind: GKTurnBasedMatch)

Handles when the view controller finds participants for a turn-based match.

Deprecated

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, playerQuitFor: GKTurnBasedMatch)

Handles when a player quits the match.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the Delegate

var turnBasedMatchmakerDelegate: (any GKTurnBasedMatchmakerViewControllerDelegate)?

The object that handles turn-based matchmaker view controller changes.

