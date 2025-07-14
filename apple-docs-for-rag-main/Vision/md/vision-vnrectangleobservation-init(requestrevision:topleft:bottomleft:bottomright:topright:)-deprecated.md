

- Vision
- VNRectangleObservation
-  init(requestRevision:topLeft:bottomLeft:bottomRight:topRight:) Deprecated

Initializer

# init(requestRevision:topLeft:bottomLeft:bottomRight:topRight:)

Creates a rectangle observation from its corner points.

iOS 13.0–17.0DeprecatediPadOS 13.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.15–14.0DeprecatedtvOS 13.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init(
    requestRevision: Int,
    topLeft: CGPoint,
    bottomLeft: CGPoint,
    bottomRight: CGPoint,
    topRight: CGPoint
)
```

Deprecated

Use init(requestRevision:topLeft:topRight:bottomRight:bottomLeft:) instead.

## Parameters 

`requestRevision`  

The rectangle detector revision number. A higher revision indicates more recent iterations of the framework.

`topLeft`  

The upper-left corner point.

`bottomLeft`  

The lower-left corner point.

`bottomRight`  

The lower-right corner point.

`topRight`  

The upper-right corner point.

## See Also

### Creating an Observation

convenience init(requestRevision: Int, topLeft: CGPoint, topRight: CGPoint, bottomRight: CGPoint, bottomLeft: CGPoint)

Creates a rectangle observation from its corner points.

