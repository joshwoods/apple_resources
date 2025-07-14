

- Game Controller
- GCMotion
-  setUserAcceleration(\_:) 

Instance Method

# setUserAcceleration(\_:)

Sets the acceleration the user applies to the controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setUserAcceleration(_ userAcceleration: GCAcceleration)
```

## Parameters 

`userAcceleration`  

The acceleration that the user applies.

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

func setGravity(GCAcceleration)

Sets the controller’s gravity data.

