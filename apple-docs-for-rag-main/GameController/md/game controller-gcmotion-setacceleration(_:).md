

- Game Controller
- GCMotion
-  setAcceleration(\_:) 

Instance Method

# setAcceleration(\_:)

Sets the total acceleration of the controller that includes gravity and the user’s acceleration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func setAcceleration(_ acceleration: GCAcceleration)
```

## Parameters 

`acceleration`  

The total acceleration of the controller.

## See Also

### Setting Snapshot Values

func setStateFrom(GCMotion)

Copies the input values from a specified motion profile to a snapshot of a motion profile.

func setAttitude(GCQuaternion)

Sets the controller’s attitude.

func setRotationRate(GCRotationRate)

Sets the controller’s rotation rate.

func setGravity(GCAcceleration)

Sets the controller’s gravity data.

func setUserAcceleration(GCAcceleration)

Sets the acceleration the user applies to the controller.

