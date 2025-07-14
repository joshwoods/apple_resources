

- TipKit
- TipUICollectionViewCell
-  configureTip(\_:arrowEdge:actionHandler:) 

Instance Method

# configureTip(\_:arrowEdge:actionHandler:)

Configures the cell to display an embedded tip view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@discardableResult @MainActor @preconcurrency
final func configureTip(
    _ tip: any Tip,
    arrowEdge: Edge? = nil,
    actionHandler: @escaping (Tips.Action) -> Void = { _ in }
) -> Self
```

## Parameters 

`tip`  

The tip to display.

`arrowEdge`  

The edge of the tip view that displays the arrow.

`actionHandler`  

The closure to perform when the user triggers a tip’s action.

## Return Value

A collection cell view that embeds the specified tip.

