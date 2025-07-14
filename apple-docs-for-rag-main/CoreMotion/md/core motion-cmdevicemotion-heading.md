

- Core Motion
- CMDeviceMotion
-  heading 

Instance Property

# heading

The heading angle (measured in degrees) relative to the current reference frame.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+watchOS 4.0+

``` source
var heading: Double { get }
```

## Discussion

This property contains a value in the range of `0.0` to `360.0` degrees. This value is available only when the frame of reference is xMagneticNorthZVertical or xTrueNorthZVertical. If the reference frame is xArbitraryZVertical or xArbitraryCorrectedZVertical, this property contains a negative number to indicate the heading is invalid.

