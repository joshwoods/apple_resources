

- Matter
-  MTRClusterElectricalEnergyMeasurement 

Class

# MTRClusterElectricalEnergyMeasurement

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRClusterElectricalEnergyMeasurement
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAccuracy(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeCumulativeEnergyExported(with: MTRReadParams?) -> [String : Any]?

func readAttributeCumulativeEnergyImported(with: MTRReadParams?) -> [String : Any]?

func readAttributeCumulativeEnergyReset(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributePeriodicEnergyExported(with: MTRReadParams?) -> [String : Any]?

func readAttributePeriodicEnergyImported(with: MTRReadParams?) -> [String : Any]?

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

