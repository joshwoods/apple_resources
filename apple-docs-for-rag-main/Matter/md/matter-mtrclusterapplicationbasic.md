

- Matter
-  MTRClusterApplicationBasic 

Class

# MTRClusterApplicationBasic

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRClusterApplicationBasic
```

## Topics

### Initializers

init?(device: MTRDevice, endpoint: UInt16, queue: dispatch_queue_t)Deprecated

init?(device: MTRDevice, endpointID: NSNumber, queue: dispatch_queue_t)

### Instance Methods

func readAttributeAcceptedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeAllowedVendorList(with: MTRReadParams?) -> [String : Any]?

func readAttributeApplication(with: MTRReadParams?) -> [String : Any]?

func readAttributeApplicationName(with: MTRReadParams?) -> [String : Any]?

func readAttributeApplicationVersion(with: MTRReadParams?) -> [String : Any]?

func readAttributeAttributeList(with: MTRReadParams?) -> [String : Any]?

func readAttributeClusterRevision(with: MTRReadParams?) -> [String : Any]?

func readAttributeFeatureMap(with: MTRReadParams?) -> [String : Any]?

func readAttributeGeneratedCommandList(with: MTRReadParams?) -> [String : Any]?

func readAttributeProductID(with: MTRReadParams?) -> [String : Any]?

func readAttributeStatus(with: MTRReadParams?) -> [String : Any]?

func readAttributeVendorID(with: MTRReadParams?) -> [String : Any]?

func readAttributeVendorName(with: MTRReadParams?) -> [String : Any]?

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

