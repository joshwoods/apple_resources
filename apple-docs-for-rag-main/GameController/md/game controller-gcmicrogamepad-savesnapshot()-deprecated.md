

- Game Controller
- GCMicroGamepad
-  saveSnapshot() Deprecated

Instance Method

# saveSnapshot()

Saves a snapshot of all of the profile’s elements.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func saveSnapshot() -> GCMicroGamepadSnapshot
```

Deprecated

Use capture() instead.

## Return Value

A snapshot that is a copy of the controller at a moment in time, and has element values you can set.

## See Also

### Setting snapshot avlues

func setStateFrom(GCMicroGamepad)

Copies the input values from a specified micro gamepad to a snapshot of a micro gamepad.

