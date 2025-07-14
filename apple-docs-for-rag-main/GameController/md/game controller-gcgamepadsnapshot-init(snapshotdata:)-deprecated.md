

- Game Controller
- GCGamepadSnapshot
-  init(snapshotData:) Deprecated

Initializer

# init(snapshotData:)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
init(snapshotData data: Data)
```

Deprecated

Use GCExtendedGamepad instead.

## Parameters 

`data`  

A data object that contains snapshot data.

## Return Value

A new snapshot object.

## Discussion

The data format for a snapshot is private. Your snapshot object should only be created from flattened data previously obtained from a snapshot.

## See Also

### Converting Between Snapshots and Data Objects

init(controller: GCController, snapshotData: Data)

Initializes a snapshot object associated with a specific controller using a flattened data representation obtained from another snapshot.

Deprecated

var snapshotData: Data

The flattened control input values for the snapshot.

Deprecated

