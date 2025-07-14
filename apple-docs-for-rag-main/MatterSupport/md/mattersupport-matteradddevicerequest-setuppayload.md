

- MatterSupport
- MatterAddDeviceRequest
-  setupPayload 

Instance Property

# setupPayload

The payload to use for Matter device setup.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
var setupPayload: MTRSetupPayload?
```

## Overview

This is an optional field for a setup to be able to complete. If this is provided, no QR-Code selection occurs. Use of this field requires an entitlement in the application (com.apple.developer.matter.allow-setup-payload).

## See Also

### Setting up the request

struct Home

The representation of a home that appears in the picker during device setup.

struct Room

The representation of a room that appears in the picker during device setup.

struct Topology

Information describing the properties of the ecosystem.

var topology: MatterAddDeviceRequest.Topology

A configuration object representing the topology of the initiating ecosystem.

