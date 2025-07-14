

- Vision
- VNFaceObservation
-  pitch 

Instance Property

# pitch

The pitch angle of a face in radians.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var pitch: NSNumber? { get }
```

## Discussion

This value indicates the rotational angle of the face around the x-axis.

If the request doesn’t calculate the angle, the value is `nil`.

## See Also

### Determining Facial Orientation

var roll: NSNumber?

The roll angle of a face in radians.

var yaw: NSNumber?

The yaw angle of a face in radians.

