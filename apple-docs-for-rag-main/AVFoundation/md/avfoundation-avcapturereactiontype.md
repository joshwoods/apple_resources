

- AVFoundation
-  AVCaptureReactionType 

Structure

# AVCaptureReactionType

Constants that indicate the type of reaction that an effect can perform.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
struct AVCaptureReactionType
```

## Topics

### Reaction types

static let balloons: AVCaptureReactionType

A reaction that displays balloons rising through the scene.

static let confetti: AVCaptureReactionType

A reaction that displays festive spots of color falling through the scene.

static let fireworks: AVCaptureReactionType

A reaction that displays fireworks bursting in the background.

static let heart: AVCaptureReactionType

A reaction that displays one or more heart symbols.

static let lasers: AVCaptureReactionType

A reaction that displays a bright laser show projecting into the scene.

static let rain: AVCaptureReactionType

A reaction that displays a dark and stormy night.

static let thumbsUp: AVCaptureReactionType

A reaction that displays a thumbs-up symbol.

static let thumbsDown: AVCaptureReactionType

A reaction that displays a thumbs-down symbol.

### Accessing the system image name

var systemImageName: String

Returns the name of a system image that displays the recommended iconography for a specified reaction type.

### Initializers

init(rawValue: String)

Creates a reaction type with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the effect state

var reactionType: AVCaptureReactionType

The type of reaction.

var startTime: CMTime

The presentation time of the first frame where the system renders the effect.

var endTime: CMTime

The presentation time of the first frame following the end of a reaction effect.

