

- Foundation
- NSAppleEventDescriptor
-  NSAppleEventDescriptor.SendOptions 

Structure

# NSAppleEventDescriptor.SendOptions

macOS 10.11+

``` source
struct SendOptions
```

## Topics

### Constants

static var alwaysInteract: NSAppleEventDescriptor.SendOptions

static var canInteract: NSAppleEventDescriptor.SendOptions

static var canSwitchLayer: NSAppleEventDescriptor.SendOptions

static var defaultOptions: NSAppleEventDescriptor.SendOptions

static var dontAnnotate: NSAppleEventDescriptor.SendOptions

static var dontExecute: NSAppleEventDescriptor.SendOptions

static var dontRecord: NSAppleEventDescriptor.SendOptions

static var neverInteract: NSAppleEventDescriptor.SendOptions

static var noReply: NSAppleEventDescriptor.SendOptions

static var queueReply: NSAppleEventDescriptor.SendOptions

static var waitForReply: NSAppleEventDescriptor.SendOptions

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

