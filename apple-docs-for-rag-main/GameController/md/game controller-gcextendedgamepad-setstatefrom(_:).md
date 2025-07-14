

- Game Controller
- GCExtendedGamepad
-  setStateFrom(\_:) 

Instance Method

# setStateFrom(\_:)

Copies the input values from a specified extended gamepad to a snapshot of an extended gamepad.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func setStateFrom(_ extendedGamepad: GCExtendedGamepad)
```

## Parameters 

`extendedGamepad`  

The extended gamepad to copy the input values from.

## Discussion

If this extended gamepad isn’t a snapshot, this method does nothing. A snapshot is a copy of a controller at a moment in time that has element values you can set.

## See Also

### Setting snapshot values

func saveSnapshot() -> GCExtendedGamepadSnapshot

Saves a snapshot of all of the profile’s elements.

Deprecated

