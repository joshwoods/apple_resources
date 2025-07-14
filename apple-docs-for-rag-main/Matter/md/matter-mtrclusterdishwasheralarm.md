

- Matter
-  MTRClusterDishwasherAlarm 

Class

# MTRClusterDishwasherAlarm

Cluster Dishwasher Alarm Attributes and commands for configuring the Dishwasher alarm.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
class MTRClusterDishwasherAlarm
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

For all instance methods that take a completion (i.e. command invocations), the completion will be called on the provided queue.

### Instance Methods

func modifyEnabledAlarms(with: MTRDishwasherAlarmClusterModifyEnabledAlarmsParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLatch(with: MTRReadParams?) -> [String : Any]?

func readAttributeMask(with: MTRReadParams?) -> [String : Any]?

func readAttributeState(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupported(with: MTRReadParams?) -> [String : Any]?

func reset(with: MTRDishwasherAlarmClusterResetParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

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

