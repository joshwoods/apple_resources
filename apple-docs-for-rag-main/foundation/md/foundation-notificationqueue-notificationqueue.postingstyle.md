

- Foundation
- NotificationQueue
-  NotificationQueue.PostingStyle 

Enumeration

# NotificationQueue.PostingStyle

The constants that specify when notifications are posted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum PostingStyle
```

## Overview

These constants are used by the enqueue(_:postingStyle:) and enqueue(_:postingStyle:coalesceMask:forModes:) methods.

## Topics

### Constants

case asap

The notification is posted at the end of the current notification callout or timer.

case whenIdle

The notification is posted when the run loop is idle.

case now

The notification is posted immediately after coalescing.

case asap

The notification is posted at the end of the current notification callout or timer.

case whenIdle

The notification is posted when the run loop is idle.

case now

The notification is posted immediately after coalescing.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct NotificationCoalescing

The constants that specify how notifications are coalesced.

