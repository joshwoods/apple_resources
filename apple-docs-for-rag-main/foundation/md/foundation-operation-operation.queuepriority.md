

- Foundation
- Operation
-  Operation.QueuePriority 

Enumeration

# Operation.QueuePriority

These constants let you prioritize the order in which operations execute.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum QueuePriority
```

## Overview

You can use these constants to specify the relative ordering of operations that are waiting to be started in an operation queue. You should always use these constants (and not the defined value) for determining priority.

## Topics

### Constants

case veryLow

Operations receive very low priority for execution.

case low

Operations receive low priority for execution.

case normal

Operations receive the normal priority for execution.

case high

Operations receive high priority for execution.

case veryHigh

Operations receive very high priority for execution.

case veryLow

Operations receive very low priority for execution.

case low

Operations receive low priority for execution.

case normal

Operations receive the normal priority for execution.

case high

Operations receive high priority for execution.

case veryHigh

Operations receive very high priority for execution.

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

### Constants

enum QualityOfService

Constants that indicate the nature and importance of work to the system.

