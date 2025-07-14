

- UIKit
- UIApplication
-  activateSceneSession(for:errorHandler:) 

Instance Method

# activateSceneSession(for:errorHandler:)

Asks the system to activate an existing scene or create a new scene and associate it with your app.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
func activateSceneSession(
    for request: UISceneSessionActivationRequest,
    errorHandler: ((any Error) -> Void)? = nil
)
```

## Parameters 

`request`  

The activation request.

`errorHandler`  

A handler to call if the request fails.

## See Also

### Related Documentation

func requestSceneSessionActivation(UISceneSession?, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene, or create a new scene and associate it with your app.

Deprecated

### Managing a scene’s life cycle

func requestSceneSessionDestruction(UISceneSession, options: UISceneDestructionRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to dismiss an existing scene and remove it from the app switcher.

func requestSceneSessionRefresh(UISceneSession)

Asks the system to update any system UI associated with the specified scene.

struct UISceneSessionActivationRequest

A collection of properties that you use to request activation of a scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

