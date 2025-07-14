

- Matter
-  MTRXPCServerProtocol_MTRDevice 

Protocol

# MTRXPCServerProtocol_MTRDevice

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
protocol MTRXPCServerProtocol_MTRDevice : NSObjectProtocol
```

## Topics

### Instance Methods

func deviceController(UUID, nodeID: NSNumber, downloadLogOf: MTRDiagnosticLogType, timeout: TimeInterval, completion: (URL?, (any Error)?) -> Void)

func deviceController(UUID, nodeID: NSNumber, getDeviceCachePrimedWithReply: (Bool) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, getEstimatedStartTimeWithReply: (Date?) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, getEstimatedSubscriptionLatencyWithReply: (NSNumber?) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, getStateWithReply: (MTRDeviceState) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, invokeCommandWithEndpointID: NSNumber, clusterID: NSNumber, commandID: NSNumber, commandFields: Any, expectedValues: [[String : Any]]?, expectedValueInterval: NSNumber?, timedInvokeTimeout: NSNumber?, serverSideProcessingTimeout: NSNumber?, completion: MTRDeviceResponseHandler)

**Required**

func deviceController(UUID, nodeID: NSNumber, invokeCommands: [[MTRCommandWithRequiredResponse]], completion: MTRDeviceResponseHandler)

func deviceController(UUID, nodeID: NSNumber, openCommissioningWindowWithSetupPasscode: NSNumber, discriminator: NSNumber, duration: NSNumber, completion: MTRDeviceOpenCommissioningWindowHandler)

**Required**

func deviceController(UUID, nodeID: NSNumber, readAttributePaths: [MTRAttributeRequestPath], withReply: ([[String : Any]]) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, readAttributeWithEndpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, params: MTRReadParams?, withReply: ([String : Any]?) -> Void)

**Required**

func deviceController(UUID, nodeID: NSNumber, writeAttributeWithEndpointID: NSNumber, clusterID: NSNumber, attributeID: NSNumber, value: Any, expectedValueInterval: NSNumber?, timedWriteTimeout: NSNumber?)

**Required**

func downloadLog(of: MTRDiagnosticLogType, nodeID: NSNumber, timeout: TimeInterval, completion: (URL?, (any Error)?) -> Void)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTRXPCServerProtocol

