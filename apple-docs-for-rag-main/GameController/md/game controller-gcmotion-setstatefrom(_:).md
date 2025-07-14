

- Game Controller
- GCMotion
-  setStateFrom(\_:) 

Instance Method

# setStateFrom(\_:)

Copies the input values from a specified motion profile to a snapshot of a motion profile.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setStateFrom(_ motion: GCMotion)
```

## Parameters 

`motion`  

The motion profile to copy the input values from.

## See Also

### Setting Snapshot Values

func setAttitude(GCQuaternion)

Sets the controller’s attitude.

func setRotationRate(GCRotationRate)

Sets the controller’s rotation rate.

func setAcceleration(GCAcceleration)

Sets the total acceleration of the controller that includes gravity and the user’s acceleration.

func setGravity(GCAcceleration)

Sets the controller’s gravity data.

func setUserAcceleration(GCAcceleration)

Sets the acceleration the user applies to the controller.

