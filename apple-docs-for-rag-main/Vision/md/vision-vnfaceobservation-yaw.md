

- Vision
- VNFaceObservation
-  yaw 

Instance Property

# yaw

The yaw angle of a face in radians.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var yaw: NSNumber? { get }
```

## Discussion

This value indicates the rotational angle of the face around the y-axis.

If the request doesn’t calculate the angle, the value is `nil.`

## See Also

### Determining Facial Orientation

var roll: NSNumber?

The roll angle of a face in radians.

var pitch: NSNumber?

The pitch angle of a face in radians.

