

- UIKit
- UIWritingToolsCoordinator
-  init(delegate:) 

Initializer

# init(delegate:)

Creates a writing tools coordinator and assigns the specified delegate object to it.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
init(delegate: (any UIWritingToolsCoordinator.Delegate)?)
```

## Parameters 

`delegate`  

An object capable of handling Writing Tools interactions for your view. The delegate must be able to modify your view’s text storage and refresh the view’s layout and appearance.

## Discussion

Create the coordinator object during your view’s initialization, and assign the object to your view. Use the addInteraction(_:) method to add the object to your view.

