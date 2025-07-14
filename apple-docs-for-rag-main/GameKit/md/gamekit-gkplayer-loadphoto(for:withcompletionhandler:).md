

- GameKit
- GKPlayer
-  loadPhoto(for:withCompletionHandler:) 

Instance Method

# loadPhoto(for:withCompletionHandler:)

Loads a photo of the player from Game Center.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadPhoto(
    for size: GKPlayer.PhotoSize,
    withCompletionHandler completionHandler: ((UIImage?, (any Error)?) -> Void)? = nil
)
```

**macOS**

``` source
func loadPhoto(
    for size: GKPlayer.PhotoSize,
    withCompletionHandler completionHandler: ((NSImage?, (any Error)?) -> Void)? = nil
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadPhoto(for size: GKPlayer.PhotoSize) async throws -> UIImage
```

**macOS**

``` source
func loadPhoto(for size: GKPlayer.PhotoSize) async throws -> NSImage
```

## Parameters 

`size`  

A constant that determines the size of the photo to load.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

*photo*  
An image of the player. If an error occurs, this may be a cached image already on the device; otherwise, it is `nil`.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

The size of the image that returns to your game is dependent on both the size parameter and the user interface idiom of the device your game is running on.

## See Also

### Loading player photos

enum PhotoSize

The size of a photo that Game Center loads.

