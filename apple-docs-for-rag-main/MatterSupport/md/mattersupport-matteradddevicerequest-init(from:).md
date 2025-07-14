

- MatterSupport
- MatterAddDeviceRequest
-  init(from:) 

Initializer

# init(from:)

Create the request from a decoder.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

The decoder to use.

## See Also

### Creating the request

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria)

Create the request.

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria, shouldScanNetworks: Bool)

Create the request with an optional network scan.

