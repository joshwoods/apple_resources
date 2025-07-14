

- Matter
-  MTRClusterTemperatureControl 

Class

# MTRClusterTemperatureControl

Cluster Temperature Control Attributes and commands for configuring the temperature control, and reporting temperature.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterTemperatureControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxTemperature(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinTemperature(with: MTRReadParams?) -> [String : Any]?

func readAttributeSelectedTemperatureLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeStep(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedTemperatureLevels(with: MTRReadParams?) -> [String : Any]?

func readAttributeTemperatureSetpoint(with: MTRReadParams?) -> [String : Any]?

func setTemperatureWith(MTRTemperatureControlClusterSetTemperatureParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setTemperatureWithExpectedValues([[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

## Relationships

### Inherits From

- MTRGenericCluster

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

