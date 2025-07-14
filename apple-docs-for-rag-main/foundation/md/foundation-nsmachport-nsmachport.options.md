

- Foundation
- NSMachPort
-  NSMachPort.Options 

Structure

# NSMachPort.Options

Used to remove access rights to a mach port when the `NSMachPort` object is invalidated or destroyed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Constants

static var deallocateReceiveRight: NSMachPort.Options

Remove a receive right when the `NSMachPort` object is invalidated or destroyed.

static var deallocateSendRight: NSMachPort.Options

Deallocate a send right when the `NSMachPort` object is invalidated or destroyed.

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

