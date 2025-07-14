

- Matter
- MTRXPCServerProtocol_MTRDevice
-  deviceController(\_:nodeID:invokeCommandWithEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:timedInvokeTimeout:serverSideProcessingTimeout:completion:) 

Instance Method

# deviceController(\_:nodeID:invokeCommandWithEndpointID:clusterID:commandID:commandFields:expectedValues:expectedValueInterval:timedInvokeTimeout:serverSideProcessingTimeout:completion:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    invokeCommandWithEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: Any,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    timedInvokeTimeout timeout: NSNumber?,
    serverSideProcessingTimeout: NSNumber?,
    completion: @escaping MTRDeviceResponseHandler
)
```

``` source
func deviceController(
    _ controller: UUID,
    nodeID: NSNumber,
    invokeCommandWithEndpointID endpointID: NSNumber,
    clusterID: NSNumber,
    commandID: NSNumber,
    commandFields: Any,
    expectedValues: [[String : Any]]?,
    expectedValueInterval: NSNumber?,
    timedInvokeTimeout timeout: NSNumber?,
    serverSideProcessingTimeout: NSNumber?
) async throws -> [[String : Any]]
```

**Required**

