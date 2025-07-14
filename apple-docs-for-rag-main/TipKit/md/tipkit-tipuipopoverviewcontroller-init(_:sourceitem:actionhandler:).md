

- TipKit
- TipUIPopoverViewController
-  init(\_:sourceItem:actionHandler:) 

Initializer

# init(\_:sourceItem:actionHandler:)

Initializes a popover controller with the specified tip.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    _ tip: any Tip,
    sourceItem: any UIPopoverPresentationControllerSourceItem,
    actionHandler: @escaping (Tips.Action) -> Void = { _ in }
)
```

## Parameters 

`tip`  

The tip to display.

`sourceItem`  

The item on which to anchor the tip popover.

`actionHandler`  

The closure to perform when the user triggers a tip’s action.

