

- GameKit
- GKLeaderboard
-  loadImage(completionHandler:) 

Instance Method

# loadImage(completionHandler:)

Loads the image for the leaderboard.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+

**macOS**

``` source
func loadImage(completionHandler: ((NSImage?, (any Error)?) -> Void)? = nil)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)? = nil)
```

**macOS**

``` source
func loadImage() async throws -> NSImage
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
func loadImage() async throws -> UIImage
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes the request.

The block receives the following parameters:

*image*  
Contains the image for the leaderboard.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

