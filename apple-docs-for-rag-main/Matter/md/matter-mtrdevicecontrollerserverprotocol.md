

- Matter
-  MTRDeviceControllerServerProtocol 

Protocol

# MTRDeviceControllerServerProtocol

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol MTRDeviceControllerServerProtocol : NSObjectProtocol
```

## Topics

### Instance Methods

func downloadLog(withController: Any?, nodeId: NSNumber, type: MTRDiagnosticLogType, timeout: TimeInterval, completion: (String?, (any Error)?) -> Void)

func getAnyDeviceController(completion: MTRDeviceControllerGetterHandler)

**Required**

func getDeviceController(withFabricId: UInt64, completion: MTRDeviceControllerGetterHandler)Deprecated

func invokeCommand(withController: Any?, nodeId: UInt64, endpointId: NSNumber, clusterId: NSNumber, commandId: NSNumber, fields: Any, timedInvokeTimeout: NSNumber?, completion: MTRValuesHandler)

**Required**

func readAttribute(withController: Any?, nodeId: UInt64, endpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, params: [String : Any]?, completion: MTRValuesHandler)

**Required**

func readAttributeCache(withController: Any?, nodeId: UInt64, endpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, completion: MTRValuesHandler)

**Required**

func stopReports(withController: Any?, nodeId: UInt64, completion: () -> Void)

**Required**

func subscribe(withController: Any?, nodeId: UInt64, minInterval: NSNumber, maxInterval: NSNumber, params: [String : Any]?, shouldCache: Bool, completion: MTRStatusCompletion)

**Required**

func subscribeAttribute(withController: Any?, nodeId: UInt64, endpointId: NSNumber?, clusterId: NSNumber?, attributeId: NSNumber?, minInterval: NSNumber, maxInterval: NSNumber, params: [String : Any]?, establishedHandler: () -> Void)

**Required**

func writeAttribute(withController: Any?, nodeId: UInt64, endpointId: NSNumber, clusterId: NSNumber, attributeId: NSNumber, value: Any, timedWriteTimeout: NSNumber?, completion: MTRValuesHandler)

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

