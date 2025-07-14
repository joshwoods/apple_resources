

- UIKit
- UIWindow
-  init(windowScene:) 

Initializer

# init(windowScene:)

Creates a window and associates it with the specified scene object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(windowScene: UIWindowScene)
```

## Parameters 

`windowScene`  

The scene object in which to display the window.

## Return Value

A new window object associated with the specified scene.

## Discussion

This method creates the new window and automatically associates it with the specified scene. You can access this window later from the scene’s windows property.

