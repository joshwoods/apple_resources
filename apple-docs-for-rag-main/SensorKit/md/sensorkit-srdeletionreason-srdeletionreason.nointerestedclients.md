

- SensorKit
- SRDeletionReason
-  SRDeletionReason.noInterestedClients 

Case

# SRDeletionReason.noInterestedClients

Indicates that the sensor has no active stakeholders.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case noInterestedClients
```

## Discussion

The framework deletes samples for this reason when there’s been no recording activity for a particular sensor.

## See Also

### Reasons

case ageLimit

Indicates that the sample outlived the framework’s retention limit.

case lowDiskSpace

Indicates that the system’s disk space is low.

case systemInitiated

Indicates that the system requests deletion.

case userInitiated

Indicates that the user requests deletion.

