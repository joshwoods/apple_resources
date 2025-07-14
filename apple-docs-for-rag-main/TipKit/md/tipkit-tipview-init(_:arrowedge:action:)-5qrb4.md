

- TipKit
- TipView
-  init(\_:arrowEdge:action:) 

Initializer

# init(\_:arrowEdge:action:)

Creates a tip view with an optional arrow.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    _ tip: Content,
    arrowEdge: Edge? = nil,
    action: @escaping (Tips.Action) -> Void = { _ in }
)
```

## Parameters 

`tip`  

The tip to display.

`arrowEdge`  

The edge of the tip view that displays the arrow.

`action`  

The closure to perform when the user triggers a tip’s action.

## Discussion

Use a `TipView` when you want to indicate the UI element to which the tip applies, but don’t want to directly anchor the tip view to that element. Use the popoverTip(_:arrowEdge:action:) to anchor your tip to an element.

