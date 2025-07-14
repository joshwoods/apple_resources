

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.Instruction
-  RoomCaptureSession.Instruction.lowTexture 

Case

# RoomCaptureSession.Instruction.lowTexture

An instruction that indicates the framework doesn’t detect distinguishable room features.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
case lowTexture
```

## Discussion

The framework provides this instruction when:

- The user points the device at a wall with a solid color.

- The camera view finder doesn’t contain any wall edges or other defining shapes for the room.

## See Also

### Determining a coaching recommendation

case normal

An instruction that indicates scanning proceeds normally and the user needs no coaching.

case moveCloseToWall

An instruction that requests the user move closer to the wall.

case moveAwayFromWall

An instruction that requests the user move further from the wall.

case turnOnLight

An instruction that requests the user increase the amount of light in the room.

case slowDown

An instruction that requests that the user move slower.

