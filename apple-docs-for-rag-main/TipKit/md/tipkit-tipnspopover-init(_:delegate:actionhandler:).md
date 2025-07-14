

- TipKit
- TipNSPopover
-  init(\_:delegate:actionHandler:) 

Initializer

# init(\_:delegate:actionHandler:)

Initializes a popover with the specified tip.

macOS 15.0+

``` source
@MainActor @preconcurrency
required init(
    _ tip: any Tip,
    delegate: (any NSPopoverDelegate)? = nil,
    actionHandler: @escaping (Tips.Action) -> Void = { _ in }
)
```

## Parameters 

`tip`  

The tip to display.

`delegate`  

A set of optional methods that a popover delegate can implement to provide additional or custom functionality

`actionHandler`  

The closure to perform when the user triggers a tip’s action.

