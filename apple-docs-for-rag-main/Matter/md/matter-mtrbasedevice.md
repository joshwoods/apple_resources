

- Matter
-  MTRBaseDevice 

Class

# MTRBaseDevice

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRBaseDevice
```

## Topics

### Initializers

init(nodeID: NSNumber, controller: MTRDeviceController)

### Instance Properties

var sessionTransportType: MTRTransportType

### Instance Methods

func deregisterReportHandlers(with: dispatch_queue_t, completion: () -> Void)

func deregisterReportHandlers(withClientQueue: dispatch_queue_t, completion: () -> Void)Deprecated

func downloadLog(of: MTRDiagnosticLogType, timeout: TimeInterval, queue: dispatch_queue_t, completion: (URL?, (any Error)?) -> Void)

func invokeCommand(withEndpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: Any, timedInvokeTimeout: NSNumber?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func invokeCommand(withEndpointId: NSNumber, clusterId: NSNumber, commandId: NSNumber, commandFields: Any, timedInvokeTimeout: NSNumber?, clientQueue: dispatch_queue_t, completion: MTRDeviceResponseHandler)Deprecated

func openCommissioningWindow(withDiscriminator: NSNumber, duration: NSNumber, queue: dispatch_queue_t, completion: MTRDeviceOpenCommissioningWindowHandler)

func openCommissioningWindow(withSetupPasscode: NSNumber, discriminator: NSNumber, duration: NSNumber, queue: dispatch_queue_t, completion: MTRDeviceOpenCommissioningWindowHandler)

func readAttribute(withEndpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, params: MTRReadParams?, clientQueue: dispatch_queue_t, completion: MTRDeviceResponseHandler)Deprecated

func readAttributePaths([MTRAttributeRequestPath]?, eventPaths: [MTREventRequestPath]?, params: MTRReadParams?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func readAttributes(withEndpointID: NSNumber?, clusterID: NSNumber?, attributeID: NSNumber?, params: MTRReadParams?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func readEvents(withEndpointID: NSNumber?, clusterID: NSNumber?, eventID: NSNumber?, params: MTRReadParams?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func subscribe(toAttributePaths: [MTRAttributeRequestPath]?, eventPaths: [MTREventRequestPath]?, params: MTRSubscribeParams?, queue: dispatch_queue_t, reportHandler: MTRDeviceResponseHandler, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, resubscriptionScheduled: MTRDeviceResubscriptionScheduledHandler?)

func subscribe(with: dispatch_queue_t, minInterval: UInt16, maxInterval: UInt16, params: MTRSubscribeParams?, cacheContainer: MTRAttributeCacheContainer?, attributeReportHandler: MTRDeviceReportHandler?, eventReportHandler: MTRDeviceReportHandler?, errorHandler: MTRDeviceErrorHandler, subscriptionEstablished: (() -> Void)?, resubscriptionScheduled: MTRDeviceResubscriptionScheduledHandler?)Deprecated

func subscribe(with: dispatch_queue_t, params: MTRSubscribeParams, clusterStateCacheContainer: MTRClusterStateCacheContainer?, attributeReportHandler: MTRDeviceReportHandler?, eventReportHandler: MTRDeviceReportHandler?, errorHandler: MTRDeviceErrorHandler, subscriptionEstablished: MTRSubscriptionEstablishedHandler?, resubscriptionScheduled: MTRDeviceResubscriptionScheduledHandler?)

func subscribeAttribute(withEndpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, minInterval: NSNumber, maxInterval: NSNumber, params: MTRSubscribeParams?, clientQueue: dispatch_queue_t, reportHandler: MTRDeviceResponseHandler, subscriptionEstablished: (() -> Void)?)Deprecated

func subscribeToAttributes(withEndpointID: NSNumber?, clusterID: NSNumber?, attributeID: NSNumber?, params: MTRSubscribeParams?, queue: dispatch_queue_t, reportHandler: MTRDeviceResponseHandler, subscriptionEstablished: MTRSubscriptionEstablishedHandler?)

func subscribeToEvents(withEndpointID: NSNumber?, clusterID: NSNumber?, eventID: NSNumber?, params: MTRSubscribeParams?, queue: dispatch_queue_t, reportHandler: MTRDeviceResponseHandler, subscriptionEstablished: MTRSubscriptionEstablishedHandler?)

func writeAttribute(withEndpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, value: Any, timedWriteTimeout: NSNumber?, queue: dispatch_queue_t, completion: MTRDeviceResponseHandler)

func writeAttribute(withEndpointId: NSNumber, clusterId: NSNumber, attributeId: NSNumber, value: Any, timedWriteTimeout: NSNumber?, clientQueue: dispatch_queue_t, completion: MTRDeviceResponseHandler)Deprecated

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

