

- Game Controller
- GCMotion
-  setGravity(\_:) 

Instance Method

# setGravity(\_:)

Sets the controller’s gravity data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setGravity(_ gravity: GCAcceleration)
```

## Parameters 

`gravity`  

A gravity acceleration vector from the controller’s reference frame.

## See Also

### Setting Snapshot Values

func setStateFrom(GCMotion)

Copies the input values from a specified motion profile to a snapshot of a motion profile.

func setAttitude(GCQuaternion)

Sets the controller’s attitude.

func setRotationRate(GCRotationRate)

Sets the controller’s rotation rate.

func setAcceleration(GCAcceleration)

Sets the total acceleration of the controller that includes gravity and the user’s acceleration.

func setUserAcceleration(GCAcceleration)

Sets the acceleration the user applies to the controller.

