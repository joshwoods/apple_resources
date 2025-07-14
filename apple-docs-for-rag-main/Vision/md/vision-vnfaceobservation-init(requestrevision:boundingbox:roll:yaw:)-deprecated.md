

- Vision
- VNFaceObservation
-  init(requestRevision:boundingBox:roll:yaw:) Deprecated

Initializer

# init(requestRevision:boundingBox:roll:yaw:)

Creates an observation that contains the roll and yaw of the face.

iOS 12.0–15.0DeprecatediPadOS 12.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.14–12.0DeprecatedtvOS 12.0–15.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init(
    requestRevision: Int,
    boundingBox: CGRect,
    roll: NSNumber?,
    yaw: NSNumber?
)
```

Deprecated

Use init(requestRevision:boundingBox:roll:yaw:pitch:)instead.

## Parameters 

`requestRevision`  

The revision of the request.

`boundingBox`  

The bounding rectangle of the detected face landmark.

`roll`  

The rotational angle of the face landmark around the z-axis.

`yaw`  

The rotational angle of the face landmark around the y-axis.

## See Also

### Creating an Observation

convenience init(requestRevision: Int, boundingBox: CGRect, roll: NSNumber?, yaw: NSNumber?, pitch: NSNumber?)

Creates an observation that contains the roll, yaw, and pitch of the face.

