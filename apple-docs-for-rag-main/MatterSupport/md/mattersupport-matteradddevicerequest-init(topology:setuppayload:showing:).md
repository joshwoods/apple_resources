

- MatterSupport
- MatterAddDeviceRequest
-  init(topology:setupPayload:showing:) 

Initializer

# init(topology:setupPayload:showing:)

Create the request.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
init(
    topology: MatterAddDeviceRequest.Topology,
    setupPayload: MTRSetupPayload? = nil,
    showing deviceCriteria: MatterAddDeviceRequest.DeviceCriteria = .allDevices
)
```

## Parameters 

`topology`  

The topology of the home.

`setupPayload`  

The setup payload.

## See Also

### Creating the request

init(from: any Decoder) throws

Create the request from a decoder.

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria, shouldScanNetworks: Bool)

Create the request with an optional network scan.

