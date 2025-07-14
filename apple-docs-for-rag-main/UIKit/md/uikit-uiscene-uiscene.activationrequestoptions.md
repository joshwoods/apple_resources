

- UIKit
- UIScene
-  UIScene.ActivationRequestOptions 

Class

# UIScene.ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class ActivationRequestOptions
```

## Overview

Create a UIScene.ActivationRequestOptions object before you activate or create a scene using the activateSceneSession(for:errorHandler:) (Swift) or activateSceneSessionForRequest:errorHandler: (Objective-C) method of UIApplication. Use this object to specify which of your app’s existing scenes originated the request for the new scene.

## Topics

### Specifying the originator of the request

var requestingScene: UIScene?

The scene object that requested the activation of a different scene.

### Specifying collection join behavior

var collectionJoinBehavior: UISceneCollectionJoinBehavior

The behavior that specifies how a new scene joins a scene collection.

enum UISceneCollectionJoinBehavior

A set of behaviors that specify how a new scene joins a scene collection.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIWindowScene.ActivationRequestOptions

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

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

