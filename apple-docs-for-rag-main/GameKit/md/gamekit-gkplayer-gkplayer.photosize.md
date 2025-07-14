

- GameKit
- GKPlayer
-  GKPlayer.PhotoSize 

Enumeration

# GKPlayer.PhotoSize

The size of a photo that Game Center loads.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
enum PhotoSize
```

## Topics

### Constants

case small

Loads a small photo.

case normal

Loads a normal-sized photo.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Loading player photos

func loadPhoto(for: GKPlayer.PhotoSize, withCompletionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads a photo of the player from Game Center.

