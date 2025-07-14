

- UIKit
- UIScene
-  init(session:connectionOptions:) 

Initializer

# init(session:connectionOptions:)

Creates a scene object using the specified session and connection information.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    session: UISceneSession,
    connectionOptions: UIScene.ConnectionOptions
)
```

## Parameters 

`session`  

A session object containing the configuration details for the scene. The system creates the session object and passes it to this initialization method.

`connectionOptions`  

An object containing additional options for connecting the scene to your app.

## Return Value

An initialized scene object.

## Discussion

Subclasses call this method to initialize the scene details.

