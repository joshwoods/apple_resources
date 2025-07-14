

- Game Controller
- GCMotion
-  setAttitude(\_:) 

Instance Method

# setAttitude(\_:)

Sets the controller’s attitude.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setAttitude(_ attitude: GCQuaternion)
```

## Parameters 

`attitude`  

The orientation of a body relative to the controller’s reference frame.

## See Also

### Setting Snapshot Values

func setStateFrom(GCMotion)

Copies the input values from a specified motion profile to a snapshot of a motion profile.

func setRotationRate(GCRotationRate)

Sets the controller’s rotation rate.

func setAcceleration(GCAcceleration)

Sets the total acceleration of the controller that includes gravity and the user’s acceleration.

func setGravity(GCAcceleration)

Sets the controller’s gravity data.

func setUserAcceleration(GCAcceleration)

Sets the acceleration the user applies to the controller.

