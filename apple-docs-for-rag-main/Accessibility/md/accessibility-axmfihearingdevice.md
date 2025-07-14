

- Accessibility
-  AXMFiHearingDevice 

Structure

# AXMFiHearingDevice

A namespace for hearing device accessibility symbols in Swift.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct AXMFiHearingDevice
```

## Topics

### Streaming status

static func streamingEar() -> AXMFiHearingDevice.Ear

Returns which ears enable streaming.

struct Ear

Constants that represent a hearing device ear.

static let streamingEarDidChangeNotification: NSNotification.Name

A notification that the system posts when there’s a change to which ears enable streaming.

### Streaming type

static func supportsBidirectionalStreaming() -> Bool

Returns a Boolean value that indicates whether the iOS device supports bidirectional streaming.

### Paired hearing devices

static func pairedDeviceIdentifiers() -> [UUID]

Returns the UUIDs of the hearing device peripherals.

static let pairedUUIDsDidChangeNotification: NSNotification.Name

A notification that the system posts when there’s a change to the UUIDs of the hearing device peripherals.

## Relationships

### Conforms To

- BitwiseCopyable

