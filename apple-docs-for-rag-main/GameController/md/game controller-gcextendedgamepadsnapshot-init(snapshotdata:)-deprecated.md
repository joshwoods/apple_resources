

- Game Controller
- GCExtendedGamepadSnapshot
-  init(snapshotData:) Deprecated

Initializer

# init(snapshotData:)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init(snapshotData data: Data)
```

Deprecated

Use the withExtendedGamepad() method instead.

## Parameters 

`data`  

A data object that contains snapshot data.

## Return Value

A new snapshot object.

## Discussion

The data format for a snapshot is private. Your snapshot object should only be created from flattened data previously obtained from an extended snapshot.

## See Also

### Converting Between Extended Snapshots and Data Objects

init(controller: GCController, snapshotData: Data)

Initializes a snapshot object associated with a specific controller using a flattened data representation obtained from another snapshot.

Deprecated

var snapshotData: Data

Flattens a snapshot into an archivable memory representation.

Deprecated

