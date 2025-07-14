

- Foundation
- NotificationQueue
-  NotificationQueue.NotificationCoalescing 

Structure

# NotificationQueue.NotificationCoalescing

The constants that specify how notifications are coalesced.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NotificationCoalescing
```

## Overview

These constants are used by the enqueue(_:postingStyle:coalesceMask:forModes:) method.

## Topics

### Constants

static var none: NotificationQueue.NotificationCoalescing

Do not coalesce notifications in the queue.

static var onName: NotificationQueue.NotificationCoalescing

Coalesce notifications with the same name.

static var onSender: NotificationQueue.NotificationCoalescing

Coalesce notifications with the same object.

static var none: NotificationQueue.NotificationCoalescing

Do not coalesce notifications in the queue.

static var onName: NotificationQueue.NotificationCoalescing

Coalesce notifications with the same name.

static var onSender: NotificationQueue.NotificationCoalescing

Coalesce notifications with the same object.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

enum PostingStyle

The constants that specify when notifications are posted.

