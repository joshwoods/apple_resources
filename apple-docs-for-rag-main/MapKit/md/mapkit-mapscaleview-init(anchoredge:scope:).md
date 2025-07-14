

- MapKit
- MapScaleView
-  init(anchorEdge:scope:) 

Initializer

# init(anchorEdge:scope:)

Creates a map scale view.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
@MainActor @preconcurrency
init(
    anchorEdge: HorizontalEdge = .leading,
    scope: Namespace.ID? = nil
)
```

## Parameters 

`anchorEdge`  

The fixed edge the scale grows and shrinks from. Use this outside of `Map/mapControls(_:)` view modifier.

`scope`  

A Namespace.ID value that identifies this namespace and that you can use to associate this control with a map instance.

