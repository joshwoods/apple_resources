

- Accessibility
- AXMFiHearingDevice
-  pairedUUIDsDidChangeNotification 

Type Property

# pairedUUIDsDidChangeNotification

A notification that the system posts when there’s a change to the UUIDs of the hearing device peripherals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let pairedUUIDsDidChangeNotification: NSNotification.Name
```

## Discussion

The system posts this notification when the value of pairedDeviceIdentifiers() changes.

## See Also

### Paired hearing devices

static func pairedDeviceIdentifiers() -> [UUID]

Returns the UUIDs of the hearing device peripherals.

