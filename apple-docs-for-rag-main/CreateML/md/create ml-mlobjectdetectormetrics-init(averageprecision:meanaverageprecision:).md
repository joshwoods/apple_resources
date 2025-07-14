

- Create ML
- MLObjectDetectorMetrics
-  init(averagePrecision:meanAveragePrecision:) 

Initializer

# init(averagePrecision:meanAveragePrecision:)

Creates metrics for an object detector given an average precision and a mean average precision.

macOS 10.15+

``` source
init(
    averagePrecision: (variedIoU: [String : Double], IoU50: [String : Double]),
    meanAveragePrecision: (variedIoU: Double, IoU50: Double)
)
```

## Parameters 

`averagePrecision`  

The `averagePrecision` for this `MLObjectDetectorMetrics`.

`meanAveragePrecision`  

The `meanAveragePrecision` for this `MLObjectDetectorMetrics`.

## Discussion

You do not use this initializer. Create ML uses this initializer to generate metrics for you when train an object detector or when you use an evaluation method.

