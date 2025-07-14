

- Game Controller
-  GCExtendedGamepadSnapShotDataV100FromNSData(\_:\_:) Deprecated

Function

# GCExtendedGamepadSnapShotDataV100FromNSData(\_:\_:)

Copies the recorded data from an extended gamepad snapshot into a readable structure.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func GCExtendedGamepadSnapShotDataV100FromNSData(
    _ snapshotData: UnsafeMutablePointer?,
    _ data: Data?
) -> Bool
```

Deprecated

Use the GCExtendedGamepad class instead.

## Parameters 

`snapshotData`  

A pointer to memory to fill with the shapshot data.

`data`  

An NSData object that contains recorded data. Often, this is obtained by calling the snapshotData method of a GCExtendedGamepadSnapshot object.

## Return Value

true if the data could be copied, false if `snapshotData` is `nil`, `data` is `nil`, or if the contents of `data` do not contain a compatible snapshot.

## See Also

### Flattening a Snapshot to Memory

struct GCExtendedGamepadSnapShotDataV100

A structure that holds a snapshot of an extended gamepad controller’s input data.

Deprecated

func NSDataFromGCExtendedGamepadSnapShotDataV100(UnsafeMutablePointer&lt;GCExtendedGamepadSnapShotDataV100>?) -> Data?

Encapsulates the controller data from an extended gamepad structure into a data object.

Deprecated

