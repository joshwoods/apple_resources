

- UIKit
- UIApplication
-  requestSceneSessionRefresh(\_:) 

Instance Method

# requestSceneSessionRefresh(\_:)

Asks the system to update any system UI associated with the specified scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func requestSceneSessionRefresh(_ sceneSession: UISceneSession)
```

## Parameters 

`sceneSession`  

The session whose scene you want to update.

## Discussion

Call this method when your scene is in the background and any part of your scene’s visible appearance changes. For example, call this method after updating your scene’s content to let the system know your scene’s snapshot requires refreshing. You don’t need to call this method when your scene is running in the foreground.

## See Also

### Managing a scene’s life cycle

func activateSceneSession(for: UISceneSessionActivationRequest, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene or create a new scene and associate it with your app.

func requestSceneSessionDestruction(UISceneSession, options: UISceneDestructionRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to dismiss an existing scene and remove it from the app switcher.

struct UISceneSessionActivationRequest

A collection of properties that you use to request activation of a scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

