

- UIKit
- UIContextMenuInteraction
-  init(delegate:) 

Initializer

# init(delegate:)

Creates a context menu interaction object with the specified delegate object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
init(delegate: any UIContextMenuInteractionDelegate)
```

## Parameters 

`delegate`  

The object that provides the contextual menu and responds to other interaction-related events. This object must adopt the UIContextMenuInteractionDelegate protocol.

## Return Value

A new context menu interaction object with the associated delegate.

## See Also

### Creating a context menu interaction object

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

