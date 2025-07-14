

- Foundation
- Process
-  Process.TerminationReason 

Enumeration

# Process.TerminationReason

Constants that specify the termination reason values that the system returns.

macOS 10.6+

``` source
enum TerminationReason
```

## Topics

### Constants

case exit

The task exited normally.

case uncaughtSignal

The task exited due to an uncaught signal.

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

