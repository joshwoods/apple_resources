

- Create ML Components
- RobustScaler
-  init(quantileRange:) 

Initializer

# init(quantileRange:)

Creates a robust scaler.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(quantileRange: ClosedRange = 0.25...0.75)
```

## Parameters 

`quantileRange`  

This scaler removes the median and scales the data according to the quantile range.

