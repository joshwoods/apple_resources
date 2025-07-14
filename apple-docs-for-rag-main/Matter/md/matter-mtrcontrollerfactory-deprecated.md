

- Matter
-  MTRControllerFactory Deprecated

Class

# MTRControllerFactory

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class MTRControllerFactory
```

Deprecated

Please use MTRDeviceControllerFactory

## Topics

### Instance Properties

var isRunning: Bool

### Instance Methods

func shutdown()

func startController(onExistingFabric: MTRDeviceControllerStartupParams) -> MTRDeviceController?

func startController(onNewFabric: MTRDeviceControllerStartupParams) -> MTRDeviceController?

func startup(MTRControllerFactoryParams) -> Bool

### Type Methods

class func sharedInstance() -> MTRControllerFactory

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

