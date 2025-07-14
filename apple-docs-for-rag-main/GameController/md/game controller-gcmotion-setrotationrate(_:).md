

- Game Controller
- GCMotion
-  setRotationRate(\_:) 

Instance Method

# setRotationRate(\_:)

Sets the controller’s rotation rate.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setRotationRate(_ rotationRate: GCRotationRate)
```

## Parameters 

`rotationRate`  

A gyroscopic measurement of the controller’s rotation around the x, y, and z axes.

## See Also

### Setting Snapshot Values

func setStateFrom(GCMotion)

Copies the input values from a specified motion profile to a snapshot of a motion profile.

func setAttitude(GCQuaternion)

Sets the controller’s attitude.

func setAcceleration(GCAcceleration)

Sets the total acceleration of the controller that includes gravity and the user’s acceleration.

func setGravity(GCAcceleration)

Sets the controller’s gravity data.

func setUserAcceleration(GCAcceleration)

Sets the acceleration the user applies to the controller.

