

- Game Controller
- GCExtendedGamepadSnapshot
-  snapshotData Deprecated

Instance Property

# snapshotData

Flattens a snapshot into an archivable memory representation.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var snapshotData: Data { get set }
```

Deprecated

Use the withExtendedGamepad() method instead.

## Discussion

You can assign another NSData object containing extended snapshot data to this property. The elements of the extended snapshot are updated to the values stored in the flattened data. This triggers any value handlers attached to those elements.

## See Also

### Converting Between Extended Snapshots and Data Objects

init(snapshotData: Data)

Initializes a snapshot object with the flattened data representation obtained from another snapshot.

Deprecated

init(controller: GCController, snapshotData: Data)

Initializes a snapshot object associated with a specific controller using a flattened data representation obtained from another snapshot.

Deprecated

