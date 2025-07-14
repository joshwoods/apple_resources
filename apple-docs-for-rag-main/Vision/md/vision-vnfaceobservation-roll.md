

- Vision
- VNFaceObservation
-  roll 

Instance Property

# roll

The roll angle of a face in radians.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var roll: NSNumber? { get }
```

## Discussion

This value indicates the rotational angle of the face around the z-axis.

If the request doesn’t calculate the angle, the value is `nil`.

## See Also

### Determining Facial Orientation

var yaw: NSNumber?

The yaw angle of a face in radians.

var pitch: NSNumber?

The pitch angle of a face in radians.

