

- Matter
-  MTRClusterBasicInformation 

Class

# MTRClusterBasicInformation

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRClusterBasicInformation
```

## Topics

### Initializers

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeCapabilityMinima(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeDataModelRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeHardwareVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeHardwareVersionString(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocalConfigDisabled(with: MTRReadParams?) -> [String : Any]?

func readAttributeLocation(with: MTRReadParams?) -> [String : Any]?

func readAttributeManufacturingDate(with: MTRReadParams?) -> [String : Any]?

func readAttributeNodeLabel(with: MTRReadParams?) -> [String : Any]?

func readAttributePartNumber(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductAppearance(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductID(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductLabel(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductName(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductURL(with: MTRReadParams?) -> [String : Any]?

func readAttributeReachable(with: MTRReadParams?) -> [String : Any]?

func readAttributeSerialNumber(with: MTRReadParams?) -> [String : Any]?

func readAttributeSoftwareVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeSoftwareVersionString(with: MTRReadParams?) -> [String : Any]?

func readAttributeUniqueID(with: MTRReadParams?) -> [String : Any]?

func readAttributeVendorID(with: MTRReadParams?) -> [String : Any]?

func readAttributeVendorName(with: MTRReadParams?) -> [String : Any]?

func writeAttributeLocalConfigDisabled(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLocalConfigDisabled(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeLocation(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeLocation(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func writeAttributeNodeLabel(withValue: [String : Any], expectedValueInterval: NSNumber)

func writeAttributeNodeLabel(withValue: [String : Any], expectedValueInterval: NSNumber, params: MTRWriteParams?)

func readAttributeMaxPathsPerInvoke(with: MTRReadParams?) -> [String : Any]?

func readAttributeSpecificationVersion(with: MTRReadParams?) -> [String : Any]?

## Relationships

### Inherits From

- MTRGenericCluster

### Inherited By

- MTRClusterBasic

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

