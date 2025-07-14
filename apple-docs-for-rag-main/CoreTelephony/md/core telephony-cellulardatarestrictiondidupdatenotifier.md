

- Core Telephony
-  CellularDataRestrictionDidUpdateNotifier 

Type Alias

# CellularDataRestrictionDidUpdateNotifier

A block to provide updates on the app’s cellular data restriction state.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.10+

``` source
typealias CellularDataRestrictionDidUpdateNotifier = (CTCellularDataRestrictedState) -> Void
```

## See Also

### Handling Policy Changes

var cellularDataRestrictionDidUpdateNotifier: CellularDataRestrictionDidUpdateNotifier?

A block that handles cellular data restriction state changes.

