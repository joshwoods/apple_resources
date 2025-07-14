

- GameKit
- GKMatchmaker
-  stopBrowsingForNearbyPlayers() 

Instance Method

# stopBrowsingForNearbyPlayers()

Stops finding nearby players.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func stopBrowsingForNearbyPlayers()
```

## Discussion

If you use the startBrowsingForNearbyPlayers(handler:) method to find nearby players, call this method when you are done.

## See Also

### Looking for nearby players

func startBrowsingForNearbyPlayers(handler: ((GKPlayer, Bool) -> Void)?)

Finds nearby players through Bluetooth or WiFi on the same subnet.

