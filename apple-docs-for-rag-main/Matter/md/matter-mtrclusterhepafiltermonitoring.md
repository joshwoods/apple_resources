

- Matter
-  MTRClusterHEPAFilterMonitoring 

Class

# MTRClusterHEPAFilterMonitoring

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterHEPAFilterMonitoring
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeChangeIndication(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCondition(with: MTRReadParams?) -> [String : Any]?

func readAttributeDegradationDirection(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeInPlaceIndicator(with: MTRReadParams?) -> [String : Any]?

func readAttributeLastChangedTime(with: MTRReadParams?) -> [String : Any]?

func readAttributeReplacementProductList(with: MTRReadParams?) -> [String : Any]?

func resetCondition(with: MTRHEPAFilterMonitoringClusterResetConditionParams?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func resetCondition(withExpectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeLastChangedTime(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLastChangedTime(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

