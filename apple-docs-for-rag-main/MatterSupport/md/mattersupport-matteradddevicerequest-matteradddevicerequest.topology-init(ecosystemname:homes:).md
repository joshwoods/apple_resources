

- MatterSupport
- MatterAddDeviceRequest
- MatterAddDeviceRequest.Topology
-  init(ecosystemName:homes:) 

Initializer

# init(ecosystemName:homes:)

Creates the topology.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
init(
    ecosystemName: String,
    homes: [MatterAddDeviceRequest.Home]
)
```

## Parameters 

`ecosystemName`  

The name of your ecosystem. This is a localized string that appears during device setup.

`homes`  

An array of available homes to add the new device into.

## See Also

### Creating the topology

init(from: any Decoder) throws

Create the request from a decoder.

