

- SwiftUI
- UnitCurve
-  value(at:) 

Instance Method

# value(at:)

Returns the output value (y component) of the curve at the given time.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func value(at progress: Double) -> Double
```

## Return Value

The output value (y component) of the curve at the given progress.

## See Also

### Getting curve characteristics

func velocity(at: Double) -> Double

Returns the rate of change (first derivative) of the output value of the curve at the given time.

