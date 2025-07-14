

- MatterSupport
-  MatterAddDeviceRequest 

Structure

# MatterAddDeviceRequest

A request that adds and sets up a device into an ecosystem.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct MatterAddDeviceRequest
```

## Topics

### Creating the request

init(from: any Decoder) throws

Create the request from a decoder.

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria)

Create the request.

init(topology: MatterAddDeviceRequest.Topology, setupPayload: MTRSetupPayload?, showing: MatterAddDeviceRequest.DeviceCriteria, shouldScanNetworks: Bool)

Create the request with an optional network scan.

### Setting up the request

struct Home

The representation of a home that appears in the picker during device setup.

struct Room

The representation of a room that appears in the picker during device setup.

struct Topology

Information describing the properties of the ecosystem.

var setupPayload: MTRSetupPayload?

The payload to use for Matter device setup.

var topology: MatterAddDeviceRequest.Topology

A configuration object representing the topology of the initiating ecosystem.

### Defining the device criteria

enum DeviceCriteria

A predicate to match against possible devices that may appear in the picker.

var showDeviceCriteria: MatterAddDeviceRequest.DeviceCriteria

A predicate that filters what devices appear in the picker.

### Performing the request

var shouldScanNetworks: Bool

A flag that indicates whether to receive network scan results.

func perform() async throws

Launch the user interface to set up a Matter device in the ecosystem.

### Type Properties

static var isSupported: Bool

A flag that indicates whether `MatterAddDeviceRequest` usage is supported

### Default Implementations

Decodable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Adding a device

Adding Matter support to your ecosystem

Allow people to add Matter accessories to your platform.

class MatterAddDeviceExtensionRequestHandler

The object that handles configuration and commissioning of a device into an ecosystem.

