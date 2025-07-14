

- Matter
-  MTRClusterRadonConcentrationMeasurement 

Class

# MTRClusterRadonConcentrationMeasurement

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterRadonConcentrationMeasurement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageMeasuredValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeAverageMeasuredValueWindow(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeLevelValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeMaxMeasuredValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasuredValue(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasurementMedium(with: MTRReadParams?) -> [String : Any]?

func readAttributeMeasurementUnit(with: MTRReadParams?) -> [String : Any]?

func readAttributeMinMeasuredValue(with: MTRReadParams?) -> [String : Any]?

func readAttributePeakMeasuredValue(with: MTRReadParams?) -> [String : Any]?

func readAttributePeakMeasuredValueWindow(with: MTRReadParams?) -> [String : Any]?

func readAttributeUncertainty(with: MTRReadParams?) -> [String : Any]?

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

