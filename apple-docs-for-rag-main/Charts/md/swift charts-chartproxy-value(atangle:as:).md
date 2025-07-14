

- Swift Charts
- ChartProxy
-  value(atAngle:as:) 

Instance Method

# value(atAngle:as:)

Returns the data value at the given angle, or `nil` if the angle does not correspond to a valid data value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func value(
    atAngle angle: Angle,
    as: P.Type = P.self
) -> P? where P : Plottable
```

## Parameters 

`angle`  

The angle, relative to the plot center, where the 12 o’clock position is interpreted as zero degrees, increasing clockwise.

## Return Value

The data value at the given position.

