

- MatterSupport
- MatterAddDeviceRequest
-  init(topology:setupPayload:showing:shouldScanNetworks:) 

Initializer

# init(topology:setupPayload:showing:shouldScanNetworks:)

Create the request with an optional network scan.

iOS 16.4+iPadOS 16.4+Mac CatalystmacOS 14.0+visionOS

``` source
init(
    topology: MatterAddDeviceRequest.Topology,
    setupPayload: MTRSetupPayload? = nil,
    showing deviceCriteria: MatterAddDeviceRequest.DeviceCriteria = .allDevices,
    shouldScanNetworks: Bool = true
)
```

## Parameters 

`topology`  

The topology of the home.

`setupPayload`  

The setup payload.

`shouldScanNetworks`  

A flag that determines whether to request a network scan.

## See Also

### Creating the request

init(from: any Decoder) throws

Create the request from a decoder.

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria)

Create the request.

