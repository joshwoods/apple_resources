

- Vision
- VNRectangleObservation
-  init(requestRevision:topLeft:topRight:bottomRight:bottomLeft:) 

Initializer

# init(requestRevision:topLeft:topRight:bottomRight:bottomLeft:)

Creates a rectangle observation from its corner points.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init(
    requestRevision: Int,
    topLeft: CGPoint,
    topRight: CGPoint,
    bottomRight: CGPoint,
    bottomLeft: CGPoint
)
```

## Parameters 

`requestRevision`  

The rectangle detector revision number. A higher revision indicates more recent iterations of the framework.

`topLeft`  

The upper-left corner point.

`topRight`  

The upper-right corner point.

`bottomRight`  

The lower-right corner point.

`bottomLeft`  

The lower-left corner point.

## See Also

### Creating an Observation

convenience init(requestRevision: Int, topLeft: CGPoint, bottomLeft: CGPoint, bottomRight: CGPoint, topRight: CGPoint)

Creates a rectangle observation from its corner points.

Deprecated

