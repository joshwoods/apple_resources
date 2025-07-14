

- Game Controller
- GCPhysicalInputProfile
-  capture() 

Instance Method

# capture()

Returns a snapshot of the profile with its current element values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func capture() -> Self
```

## Return Value

A snapshot of the profile.

## Discussion

A snapshot is a copy of profile at a moment in time with its current element values. Unlike other profiles, you can set the values of a snapshot’s elements.

## See Also

### Setting snapshot values

func setStateFromPhysicalInput(GCPhysicalInputProfile)

Copies the input values from a specified physical input profile to a snapshot of the profile.

