

- UIKit
-  UISceneWindowingBehaviors 

Class

# UISceneWindowingBehaviors

An object with properties that determine the behavior of a window.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
class UISceneWindowingBehaviors
```

## Topics

### Specifying window behaviors

var isClosable: Bool

A Boolean value that determines whether the window displays a close button.

var isMiniaturizable: Bool

A Boolean value that determines whether the window displays a minimize button.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Determining window behaviors

var isFullScreen: Bool

A Boolean value that indicates whether the window scene is full screen or windowed.

var windowingBehaviors: UISceneWindowingBehaviors?

An object that specifies the behaviors of the window.

