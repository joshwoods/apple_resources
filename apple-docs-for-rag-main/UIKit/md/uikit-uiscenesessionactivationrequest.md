

- UIKit
-  UISceneSessionActivationRequest 

Structure

# UISceneSessionActivationRequest

A collection of properties that you use to request activation of a scene.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
struct UISceneSessionActivationRequest
```

## Overview

A `UISceneSessionActiviationRequest` object provides information about how to activate a scene session. Create a request to specify:

- A user activity for the scene session.

- An existing scene session.

- A scene session with a specific role.

You create a `UISceneSessionActivationRequest` object in your code, then you pass it as a parameter when you call activateSceneSession(for:errorHandler:) to ask the system to activate the scene session.

## Topics

### Creating a request

init(role: UISceneSession.Role, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?)

Creates a scene session activation request object with a role, a user activity, and options that you provide.

init(session: UISceneSession, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?)

Creates a scene session activation request object with a scene session, a user activity, and options that you provide.

### Managing request details

var options: UIScene.ActivationRequestOptions?

Activation request options to further customize the request.

var role: UISceneSession.Role

The role to request.

var session: UISceneSession?

The specific scene session to activate.

var userActivity: NSUserActivity?

A user activity to send to the newly activated scene.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Managing a scene’s life cycle

func activateSceneSession(for: UISceneSessionActivationRequest, errorHandler: ((any Error) -> Void)?)

Asks the system to activate an existing scene or create a new scene and associate it with your app.

func requestSceneSessionDestruction(UISceneSession, options: UISceneDestructionRequestOptions?, errorHandler: ((any Error) -> Void)?)

Asks the system to dismiss an existing scene and remove it from the app switcher.

func requestSceneSessionRefresh(UISceneSession)

Asks the system to update any system UI associated with the specified scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating the session associated with a scene.

class UISceneDestructionRequestOptions

An object you pass to UIKit to permanently remove a scene and its associated session from your app.

