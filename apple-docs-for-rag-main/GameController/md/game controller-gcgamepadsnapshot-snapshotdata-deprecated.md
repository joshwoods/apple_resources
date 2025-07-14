

- Game Controller
- GCGamepadSnapshot
-  snapshotData Deprecated

Instance Property

# snapshotData

The flattened control input values for the snapshot.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var snapshotData: Data { get set }
```

Deprecated

Use the GCExtendedGamepad class instead.

## Discussion

You can assign another NSData object containing snapshot data to this property. The elements of the snapshot are updated to the values stored in the flattened data. This triggers any value handlers attached to those elements.

## See Also

### Converting Between Snapshots and Data Objects

init(snapshotData: Data)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

Deprecated

init(controller: GCController, snapshotData: Data)

Initializes a snapshot object associated with a specific controller using a flattened data representation obtained from another snapshot.

Deprecated

