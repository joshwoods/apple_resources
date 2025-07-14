

- Game Controller
- GCPhysicalInputProfile
-  setStateFromPhysicalInput(\_:) 

Instance Method

# setStateFromPhysicalInput(\_:)

Copies the input values from a specified physical input profile to a snapshot of the profile.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func setStateFromPhysicalInput(_ physicalInput: GCPhysicalInputProfile)
```

## Parameters 

`physicalInput`  

The physical input profile to copy the input values from.

## Discussion

If the associated controller isn’t a snapshot, this method does nothing.

## See Also

### Related Documentation

var isSnapshot: Bool

A Boolean value that indicates whether the controller is a snapshot of a controller.

### Setting snapshot values

func capture() -> Self

Returns a snapshot of the profile with its current element values.

