

- AppKit
- NSWritingToolsCoordinator
-  init(delegate:) 

Initializer

# init(delegate:)

Creates a writing tools coordinator and assigns the specified delegate object to it.

macOS 15.2+

``` source
@MainActor
init(delegate: (any NSWritingToolsCoordinator.Delegate)?)
```

## Parameters 

`delegate`  

An object capable of handling Writing Tools interactions for your view. The delegate must be able to modify your view’s text storage and refresh the view’s layout and appearance.

## Discussion

Create the coordinator object during your view’s initialization, and assign the object to your view. Assign the coordinator to the writingToolsCoordinator property of your view.

