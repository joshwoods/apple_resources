

- Game Controller
-  NSDataFromGCMicroGamepadSnapShotDataV100(\_:) Deprecated

Function

# NSDataFromGCMicroGamepadSnapShotDataV100(\_:)

Encapsulates the controller data from a micro gamepad structure into a data object.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func NSDataFromGCMicroGamepadSnapShotDataV100(_ snapshotData: UnsafeMutablePointer?) -> Data?
```

Deprecated

Use the withMicroGamepad() method instead.

## Parameters 

`snapshotData`  

A pointer to memory that contains a set of gamepad control values.

## Return Value

A new NSData object that contains the snapshot data, or `nil` if an error occurred.

## Discussion

If the version and size is not set in the snapshot the data will automatically have a version of `0x100` and a size equal to `sizeof(GCMicroGamepadSnapShotDataV100)`.

## See Also

### Flattening a Snapshot to Memory

struct GCMicroGamepadSnapShotDataV100

A structure that holds a snapshot of a micro gamepad controller’s input data.

Deprecated

func GCMicroGamepadSnapShotDataV100FromNSData(UnsafeMutablePointer&lt;GCMicroGamepadSnapShotDataV100>?, Data?) -> Bool

Copies the recorded data from a micro gamepad snapshot into a readable structure.

Deprecated

