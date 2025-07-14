

- Matter
-  MTRClusterBooleanStateConfiguration 

Class

# MTRClusterBooleanStateConfiguration

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterBooleanStateConfiguration
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func enableDisableAlarm(with: MTRBooleanStateConfigurationClusterEnableDisableAlarmParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAlarmsActive(with: MTRReadParams?) -> [String : Any]?

func readAttributeAlarmsEnabled(with: MTRReadParams?) -> [String : Any]?

func readAttributeAlarmsSupported(with: MTRReadParams?) -> [String : Any]?

func readAttributeAlarmsSuppressed(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCurrentSensitivityLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeDefaultSensitivityLevel(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeSensorFault(with: MTRReadParams?) -> [String : Any]?

func readAttributeSupportedSensitivityLevels(with: MTRReadParams?) -> [String : Any]?

func suppressAlarm(with: MTRBooleanStateConfigurationClusterSuppressAlarmParams, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, completion: MTRStatusCompletion)

func writeAttributeCurrentSensitivityLevel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeCurrentSensitivityLevel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

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

