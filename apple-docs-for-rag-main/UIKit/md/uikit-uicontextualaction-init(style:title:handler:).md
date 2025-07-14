

- UIKit
- UIContextualAction
-  init(style:title:handler:) 

Initializer

# init(style:title:handler:)

Creates a new contextual action with the specified title and handler.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(
    style: UIContextualAction.Style,
    title: String?,
    handler: @escaping UIContextualAction.Handler
)
```

## Parameters 

`style`  

The style information to apply to the action button.

`title`  

The title of the action button.

`handler`  

The handler to execute when the user selects the action.

## Return Value

An initialized contextual action object.

