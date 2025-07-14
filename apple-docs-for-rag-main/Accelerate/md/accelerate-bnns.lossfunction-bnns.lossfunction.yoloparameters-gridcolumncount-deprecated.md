

- Accelerate
- BNNS
- 
  - BNNS
- BNNS.LossFunction
- BNNS.LossFunction.YoloParameters
-  gridColumnCount Deprecated

Instance Property

# gridColumnCount

The number of columns in the grid.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
let gridColumnCount: Int
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Instance Properties

let anchorBoxCount: Int

The number of anchor boxes in each cell.

Deprecated

let anchorBoxSize: Int

The size of the anchor box.

Deprecated

let anchorsData: UnsafeMutablePointer&lt;Float>

Maximum IOU for treating as no object.

Deprecated

let classificationScale: Float

The value that specifies the classification scaling factor.

Deprecated

let gridRowsCount: Int

The number of rows in the grid.

Deprecated

let huberDelta: Float

A value that’s interpreted as width-height loss.

Deprecated

let noObjectMaximumIoU: Float

The value that specifies intersection over union (IOU) that’s the maximum the function treats as not an object.

Deprecated

let noObjectScale: Float

The value that specifies the no-object confidence scaling factor.

Deprecated

let objectMinimumIoU: Float

The value that specifies intersection over union (IOU) that’s the minimum the function treats as an object.

Deprecated

let objectScale: Float

The value that specifies the object confidence loss-scaling factor.

Deprecated

let rescore: Bool

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

Deprecated

let whScale: Float

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

Deprecated

let xyScale: Float

The value that specifies the x, y loss-scaling factor.

Deprecated

