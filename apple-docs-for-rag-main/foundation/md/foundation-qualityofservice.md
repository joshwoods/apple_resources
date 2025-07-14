

- Foundation
-  QualityOfService 

Enumeration

# QualityOfService

Constants that indicate the nature and importance of work to the system.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum QualityOfService
```

## Overview

Work with higher quality of service classes receive more resources than work with lower quality of service classes whenever there’s resource contention.

## Topics

### Constants

case userInteractive

case userInitiated

case utility

case background

case `default`

case userInteractive

case userInitiated

case utility

case background

case `default`

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

enum QueuePriority

These constants let you prioritize the order in which operations execute.

