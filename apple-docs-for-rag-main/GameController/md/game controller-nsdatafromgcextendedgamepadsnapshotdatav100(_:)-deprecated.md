

- Game Controller
-  NSDataFromGCExtendedGamepadSnapShotDataV100(\_:) Deprecated

Function

# NSDataFromGCExtendedGamepadSnapShotDataV100(\_:)

Encapsulates the controller data from an extended gamepad structure into a data object.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func NSDataFromGCExtendedGamepadSnapShotDataV100(_ snapshotData: UnsafeMutablePointer?) -> Data?
```

Deprecated

Use the withExtendedGamepad() method instead.

## Parameters 

`snapshotData`  

A pointer to memory that contains a set of extended gamepad control values.

## Return Value

A new NSData object that contains the snapshot data, or `nil` if an error occurred.

## Discussion

If the version and size is not set in the snapshot the data will automatically have a version of `0x100` and a size equal to `sizeof(GCExtendedGamepadSnapShotDataV100)`.

## See Also

### Flattening a Snapshot to Memory

struct GCExtendedGamepadSnapShotDataV100

A structure that holds a snapshot of an extended gamepad controller’s input data.

Deprecated

func GCExtendedGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from an extended gamepad snapshot into a readable structure.

Deprecated

