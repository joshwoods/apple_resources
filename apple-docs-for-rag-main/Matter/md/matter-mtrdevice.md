

- Matter
-  MTRDevice 

Class

# MTRDevice

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRDevice
```

## Topics

### Initializers

init(nodeID: NSNumber, controller: MTRDeviceController)

init(nodeID: UInt64, deviceController: MTRDeviceController)Deprecated

### Instance Properties

var deviceCachePrimed: Bool

var deviceController: MTRDeviceController?

var estimatedStartTime: Date?

var estimatedSubscriptionLatency: NSNumber?

var state: MTRDeviceState

var networkCommissioningFeatures: MTRNetworkCommissioningFeature

Network commissioning features supported by the device.

var productID: NSNumber?

The Product Identifier associated with the device.

var vendorID: NSNumber?

The Vendor Identifier associated with the device.

### Instance Methods

func downloadLog(of: MTRDiagnosticLogType, timeout: TimeInterval, queue: dispatch_queue_t, completion: (URL?, (any Error)?) -> Void)

func invokeCommand(withEndpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: [String : Any]?, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func invokeCommand(withEndpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: Any, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, timedInvokeTimeout: NSNumber?, clientQueue: dispatch_queue_t, completion: MTRDeviceResponseHandler)Deprecated

func invokeCommand(withEndpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: Any, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, timedInvokeTimeout: NSNumber?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func openCommissioningWindow(withDiscriminator: NSNumber, duration: NSNumber, queue: dispatch_queue_t, completion: MTRDeviceOpenCommissioningWindowHandler)

func openCommissioningWindow(withSetupPasscode: NSNumber, discriminator: NSNumber, duration: NSNumber, queue: dispatch_queue_t, completion: MTRDeviceOpenCommissioningWindowHandler)

func readAttribute(withEndpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, params: MTRReadParams?) -> [String : Any]?

func setDelegate(any MTRDeviceDelegate, queue: dispatch_queue_t)Deprecated

func writeAttribute(withEndpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, value: Any, expectedValueInterval: NSNumber, timedWriteTimeout: NSNumber?)

func add(any MTRDeviceDelegate, queue: dispatch_queue_t)

Adds a delegate to receive asynchronous callbacks about the device.

func add(any MTRDeviceDelegate, queue: dispatch_queue_t, interestedPathsForAttributes: [Any]?, interestedPathsForEvents: [Any]?)

Adds a delegate to receive asynchronous callbacks about the device, and limit attribute and/or event reports to a specific set of paths.

func descriptorClusters() -> [MTRAttributePath : [String : Any]]

Read all known attributes from descriptor clusters on all known endpoints.

func invokeCommands([[MTRCommandWithRequiredResponse]], queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

Invoke one or more groups of commands.

func readAttributePaths([MTRAttributeRequestPath]) -> [[String : Any]]

Read the attributes identified by the provided attribute paths. The paths can include wildcards.

func remove(any MTRDeviceDelegate)

Removes the delegate from receiving callbacks about the device.

func wait(forAttributeValues: [MTRAttributePath : [String : Any]], timeout: TimeInterval, queue: dispatch_queue_t, completion: ((any Error)?) -> Void) -> MTRAttributeValueWaiter

Sets up the provided completion to be called when any of the following happens:

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

