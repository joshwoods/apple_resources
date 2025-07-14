

- Accessibility
- AXMFiHearingDevice
-  AXMFiHearingDevice.Ear 

Structure

# AXMFiHearingDevice.Ear

Constants that represent a hearing device ear.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Ear
```

## Topics

### Constants

static var both: AXMFiHearingDevice.Ear

A constant that represents both ears.

static var left: AXMFiHearingDevice.Ear

A constant that represents the left ear.

static var right: AXMFiHearingDevice.Ear

A constant that represents the right ear.

### Initializer

init(rawValue: UInt)

Creates a structure that represents a hearing device ear with the raw value you specify.

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

### Streaming status

static func streamingEar() -> AXMFiHearingDevice.Ear

Returns which ears enable streaming.

static let streamingEarDidChangeNotification: NSNotification.Name

A notification that the system posts when there’s a change to which ears enable streaming.

