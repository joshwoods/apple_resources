

- ActivityKit
-  ActivityUIDismissalPolicy 

Structure

# ActivityUIDismissalPolicy

The structure that describes when the system should remove a Live Activity that ended.

iOS 16.1+iPadOS 16.1+

``` source
struct ActivityUIDismissalPolicy
```

## Topics

### Dismissing a Live Activity

static let `default`: ActivityUIDismissalPolicy

The system’s default dismissal policy for the Live Activity.

static let immediate: ActivityUIDismissalPolicy

The system immediately removes the Live Activity that ended.

static func after(Date) -> ActivityUIDismissalPolicy

The system removes the Live Activity that ended at the specified time within a four-hour window.

### Operators

static func == (ActivityUIDismissalPolicy, ActivityUIDismissalPolicy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Ending a Live Activity

func end(ActivityContent&lt;Activity&lt;Attributes>.ContentState>?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

func end(ActivityContent&lt;Activity&lt;Attributes>.ContentState>?, dismissalPolicy: ActivityUIDismissalPolicy, timestamp: Date) async

Ends an active Live Activity.

