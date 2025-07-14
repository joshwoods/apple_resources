

- Accelerate
-  BNNSCornersWidthFirst 

Global Variable

# BNNSCornersWidthFirst

Specifies coordinates as center and size with the order: width center, height center, width, height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var BNNSCornersWidthFirst: BNNSBoxCoordinateMode { get }
```

## See Also

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSCenterSizeHeightFirst: BNNSBoxCoordinateMode

Specifies coordinates as corners with the order: height start, width start, height end, width end.

var BNNSCenterSizeWidthFirst: BNNSBoxCoordinateMode

Specifies coordinates as corners with the order: width start, height start, width end, height end.

var BNNSCornersHeightFirst: BNNSBoxCoordinateMode

Specifies coordinates as center and size with the order: height center, width center, height, width.

