

- UIKit
-  UISceneDestructionRequestOptions 

Class

# UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UISceneDestructionRequestOptions
```

## Overview

Create a UISceneDestructionRequestOptions object before calling the requestSceneSessionDestruction(_:options:errorHandler:) method of UIApplication. When destroying a UIWindowScene, create a UIWindowSceneDestructionRequestOptions object instead and use it to configure the dismissal animations.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIWindowSceneDestructionRequestOptions

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing a scene’s life cycle

func activateSceneSession(for: UISceneSessionActivationRequest, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene or create a new scene and associate it with your app.

func requestSceneSessionDestruction(UISceneSession, options: UISceneDestructionRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to dismiss an existing scene and remove it from the app switcher.

func requestSceneSessionRefresh(UISceneSession)

Asks the system to update any system UI associated with the specified scene.

struct UISceneSessionActivationRequest

A collection of properties that you use to request activation of a scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

