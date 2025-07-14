

- UIKit
-  UIWindowSceneDestructionRequestOptions 

Class

# UIWindowSceneDestructionRequestOptions

An object that contains information to use when removing a window scene from your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIWindowSceneDestructionRequestOptions
```

## Overview

Create a UIWindowSceneDestructionRequestOptions object before you close one of your app’s scenes using the requestSceneSessionDestruction(_:options:errorHandler:) method of UIApplication. Use this object to specify the dismissal animations to apply to the scene’s UI, if that UI is onscreen.

## Topics

### Configuring the dismissal animation

var windowDismissalAnimation: UIWindowScene.DismissalAnimation

The animations to use when dismissing the scene’s windows.

enum DismissalAnimation

Constants that indicate the types of animations available for dismissing a scene’s windows.

## Relationships

### Inherits From

- UISceneDestructionRequestOptions

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Activation and destruction

class UISceneActivationConditions

The set of conditions that define when UIKit activates the current scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

