

- Matter
-  MTRDeviceControllerFactory 

Class

# MTRDeviceControllerFactory

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRDeviceControllerFactory
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Instance Properties

var isRunning: Bool

var knownFabrics: [MTRFabricInfo]?

### Instance Methods

func createController(onExistingFabric: MTRDeviceControllerStartupParams) throws -> MTRDeviceController

func createController(onNewFabric: MTRDeviceControllerStartupParams) throws -> MTRDeviceController

func preWarmCommissioningSession()

func start(MTRDeviceControllerFactoryParams) throws

func stop()

### Type Methods

class func sharedInstance() -> MTRDeviceControllerFactory

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

