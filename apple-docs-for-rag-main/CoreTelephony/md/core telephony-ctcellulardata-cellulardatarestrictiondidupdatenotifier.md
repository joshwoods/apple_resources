

- Core Telephony
- CTCellularData
-  cellularDataRestrictionDidUpdateNotifier 

Instance Property

# cellularDataRestrictionDidUpdateNotifier

A block that handles cellular data restriction state changes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
var cellularDataRestrictionDidUpdateNotifier: CellularDataRestrictionDidUpdateNotifier? { get set }
```

## Discussion

The system executes this block when the app first sets the callback handler, and then every time the cellular data allowed policy changes. Execution of the block occurs on the default priority global dispatch queue.

## See Also

### Handling Policy Changes

typealias CellularDataRestrictionDidUpdateNotifier

A block to provide updates on the app’s cellular data restriction state.

