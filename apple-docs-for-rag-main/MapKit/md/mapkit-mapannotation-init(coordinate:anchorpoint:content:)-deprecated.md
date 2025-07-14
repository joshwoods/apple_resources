

- MapKit
- MapAnnotation
-  init(coordinate:anchorPoint:content:) Deprecated

Initializer

# init(coordinate:anchorPoint:content:)

Creates a custom annotation that provides a SwiftUI view to display at the map location that you specify.

MapKitSwiftUIiOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac CatalystmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0DeprecatedvisionOSwatchOS 7.0–10.0Deprecated

``` source
init(
    coordinate: CLLocationCoordinate2D,
    anchorPoint: CGPoint = CGPoint(x: 0.5, y: 0.5),
    @ViewBuilder content: () -> Content
)
```

Deprecated

Use Annotation along with Map initializers that take a MapContentBuilder instead.

## Parameters 

`coordinate`  

The location of the specified annotation.

`anchorPoint`  

A CGPoint value in unit coordinate space that aligns the coordinate location of the annotation with view created. The default value `0.5`, which represents the center of the view.

`content`  

The closure that returns a custom annotation view.

## Discussion

Use the anchor point to align the SwiftUI view you return in content to the coordinate represented on the map. Anchor point uses unit coordinate space, that represents the distance between the frame edges as values between `0` and `1`. For example, to align the top-right or bottom-middle of the view with the coordinate location on the map use `CGPoint(1,0)` or `CGPoint(0.5,1)`, respectively.

