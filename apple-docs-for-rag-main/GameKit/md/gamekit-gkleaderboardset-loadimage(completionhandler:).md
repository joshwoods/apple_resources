

- GameKit
- GKLeaderboardSet
-  loadImage(completionHandler:) 

Instance Method

# loadImage(completionHandler:)

Loads the localized image that you associate with the leaderboard set.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)? = nil)
```

**macOS**

``` source
func loadImage(completionHandler: ((NSImage?, (any Error)?) -> Void)? = nil)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func loadImage() async throws -> UIImage
```

**macOS**

``` source
func loadImage() async throws -> NSImage
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes the request.

The block receives the following parameters:

*image*  
The image for the leaderboard set. If an error occurs, this property may be non-`nil` and contain data GameKit loads before the error occurs.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## See Also

### Loading Leaderboard Sets

class func loadLeaderboardSets(completionHandler: (([GKLeaderboardSet]?, (any Error)?) -> Void)?)

Loads all of the leaderboard sets you configure for your game.

func loadLeaderboards(handler: ([GKLeaderboard]?, (any Error)?) -> Void)

Loads the leaderboards in the leaderboard set.

func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads all of the leaderboards for the current leaderboard set.

Deprecated

