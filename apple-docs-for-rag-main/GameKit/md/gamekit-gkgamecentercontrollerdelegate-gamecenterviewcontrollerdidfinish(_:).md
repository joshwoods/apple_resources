

- GameKit
- GKGameCenterControllerDelegate
-  gameCenterViewControllerDidFinish(\_:) 

Instance Method

# gameCenterViewControllerDidFinish(\_:)

Handles when the player dismisses the dashboard.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func gameCenterViewControllerDidFinish(_ gameCenterViewController: GKGameCenterViewController)
```

**Required**

## Parameters 

`gameCenterViewController`  

The view controller that the player closes.

## Mentioned in 

Displaying the Game Center dashboard

## Discussion

Implement this method to dismiss the Game Center view controller. If your game paused any gameplay or other activities, this method can restart those services.

