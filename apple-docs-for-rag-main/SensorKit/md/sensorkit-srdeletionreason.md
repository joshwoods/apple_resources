

- SensorKit
-  SRDeletionReason 

Enumeration

# SRDeletionReason

Reasons that the framework deletes samples.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum SRDeletionReason
```

## Topics

### Reasons

case ageLimit

Indicates that the sample outlived the framework’s retention limit.

case lowDiskSpace

Indicates that the system’s disk space is low.

case noInterestedClients

Indicates that the sensor has no active stakeholders.

case systemInitiated

Indicates that the system requests deletion.

case userInitiated

Indicates that the user requests deletion.

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

### Accessing the Deletion Reason

var reason: SRDeletionReason

The reason the framework deletes samples.

