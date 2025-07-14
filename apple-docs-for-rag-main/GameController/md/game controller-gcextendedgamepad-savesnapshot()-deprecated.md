

- Game Controller
- GCExtendedGamepad
-  saveSnapshot() Deprecated

Instance Method

# saveSnapshot()

Saves a snapshot of all of the profile’s elements.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func saveSnapshot() -> GCExtendedGamepadSnapshot
```

Deprecated

Use the capture() method instead.

## Return Value

A snapshot that is a copy of the controller at a moment in time, and has element values you can set.

## See Also

### Setting snapshot values

func setStateFrom(GCExtendedGamepad)

Copies the input values from a specified extended gamepad to a snapshot of an extended gamepad.

