

- Matter
-  MTRClusterMicrowaveOvenControl 

Class

# MTRClusterMicrowaveOvenControl

Cluster Microwave Oven Control Attributes and commands for configuring the microwave oven control, and reporting cooking stats.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterMicrowaveOvenControl
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func addMoreTime(with: MTRMicrowaveOvenControlClusterAddMoreTimeParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCookTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxCookTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxPower(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinPower(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerSetting(with: MTRReadParams?) -> [String : Any]?

func readAttributePowerStep(with: MTRReadParams?) -> [String : Any]?

func readAttributeWattRating(with: MTRReadParams?) -> [String : Any]?

func setCookingParametersWith(MTRMicrowaveOvenControlClusterSetCookingParametersParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func setCookingParametersWithExpectedValues([[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

