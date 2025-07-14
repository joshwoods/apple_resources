

- WatchKit
-  WKSnapshotReason 

Enumeration

# WKSnapshotReason

The reason for a background snapshot task.

watchOS 4.0+

``` source
enum WKSnapshotReason
```

## Topics

### Enumeration Cases

case appBackgrounded

The app transitioned from the foreground to the background.

case appScheduled

The app scheduled this snapshot.

case complicationUpdate

The app updated the complication timeline.

case prelaunch

The system needs a snapshot for the dock, but the app has not been launched yet.

case returnToDefaultState

It has been more than an hour since the user’s last interaction with the app; the app’s snapshot should return to its default state.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Instance properties

var reasonForSnapshot: WKSnapshotReason

The reason for taking the upcoming snapshot.

var returnToDefaultState: Bool

A Boolean value indicating that the app should return to its default state.

Deprecated

