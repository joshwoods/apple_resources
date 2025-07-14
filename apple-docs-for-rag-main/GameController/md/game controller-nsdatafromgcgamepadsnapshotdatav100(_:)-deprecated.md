

- Game Controller
-  NSDataFromGCGamepadSnapShotDataV100(\_:) Deprecated

Function

# NSDataFromGCGamepadSnapShotDataV100(\_:)

Encapsulates the controller data from a gamepad structure into a data object.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func NSDataFromGCGamepadSnapShotDataV100(_ snapshotData: UnsafeMutablePointer?) -> Data?
```

Deprecated

Use the GCExtendedGamepad class instead.

## Parameters 

`snapshotData`  

A pointer to memory that contains a set of gamepad control values.

## Return Value

A new NSData object that contains the snapshot data, or `nil` if an error occurred.

## Discussion

If the version and size is not set in the snapshot the data will automatically have a version of `0x100` and a size equal to `sizeof(GCGamepadSnapShotDataV100)`.

## See Also

### Flattening a Snapshot to Memory

struct GCGamepadSnapShotDataV100

A structure that holds a snapshot of a gamepad controller’s input data.

Deprecated

func GCGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from a gamepad snapshot into a readable structure.

Deprecated

