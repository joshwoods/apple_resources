

- GameKit
- GKMatchmaker
-  startGroupActivity(playerHandler:) 

Instance Method

# startGroupActivity(playerHandler:)

Begins a SharePlay activity for your game when a FaceTime call is active.

iOS 16.2+iPadOS 16.2+Mac Catalyst 16.2+macOS 13.1+visionOS 1.0+

``` source
func startGroupActivity(playerHandler handler: @escaping (GKPlayer) -> Void)
```

## Parameters 

`handler`  

The block that GameKit calls when a person using SharePlay wants to join the group activity. GameKit invokes this handler for each player that joins until your app, or the player, stops showing the group activity in SharePlay.

This block receives the following parameter:

`player`  
A player who wants to join the group activity.

## Mentioned in 

Adding voice chat to multiplayer games

Finding multiple players for a game

## Discussion

SharePlay lets people share experiences in a group activity, such as joining your game using FaceTime or the Messages app. If you implement a custom group activity interface, use this method to show a group activity that your game provides in apps that support the SharePlay interface. For macOS apps, add the Group Activities capability to your Xcode to enable this feature.

To start a group activity on behalf of the player and receive callbacks for each player that joins, invoke the startGroupActivity(playerHandler:) method. Implement the handler to add each player that joins to the match before starting gameplay using the addPlayers(to:matchRequest:completionHandler:) method.

If an app with a SharePlay interface isn’t running when you invoke the startGroupActivity(playerHandler:) method, GameKit presents an interface that lets the player share a group activity in an app that supports SharePlay. Then the player can stop showing the group activity using the SharePlay interface, or you can stop the group activity on behalf of the player using the stopGroupActivity() method.

Alternatively, if you want to present a familiar GameKit interface, instead present a GKMatchmakerViewController object that lets the player start a group activity by selecting SharePlay to invite players.

## See Also

### Starting matches using SharePlay

func stopGroupActivity()

Ends a SharePlay activity for the entire group, which the local player activates.

