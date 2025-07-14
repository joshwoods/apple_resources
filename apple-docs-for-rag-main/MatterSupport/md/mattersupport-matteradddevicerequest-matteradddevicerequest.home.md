

- MatterSupport
- MatterAddDeviceRequest
-  MatterAddDeviceRequest.Home 

Structure

# MatterAddDeviceRequest.Home

The representation of a home that appears in the picker during device setup.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct Home
```

## Topics

### Creating the home

init(from: any Decoder) throws

Create the request from a decoder.

init(displayName: String)

Creates a new home.

### Getting the properties

var displayName: String

The name of the home that appears in the picker.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Setting up the request

struct Room

The representation of a room that appears in the picker during device setup.

struct Topology

Information describing the properties of the ecosystem.

var setupPayload: MTRSetupPayload?

The payload to use for Matter device setup.

var topology: MatterAddDeviceRequest.Topology

A configuration object representing the topology of the initiating ecosystem.

