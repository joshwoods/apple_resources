

- Network Extension
-  NEHotspotHelperCommand 

Class

# NEHotspotHelperCommand

A command for the hotspot helper to handle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEHotspotHelperCommand
```

## Overview

NEHotspostHelperCommand objects are passed to the the Hotspot Helper app’s command handler block. The Hotspot Helper app processes the command, instantiates an NEHotspotHelperResponse object, sets the annotated `network` or `networkList` (`Evaluate` or `FilterScanList` commands only), and then delivers the response to the system.

## Topics

### Command information

var commandType: NEHotspotHelperCommandType

The type of the command

enum NEHotspotHelperCommandType

var network: NEHotspotNetwork?

The network associated with the command.

var networkList: [NEHotspotNetwork]?

The list of networks associated with the command.

### Networking on the hotspot network

func bind(to: NEHotspotHelperCommand)

Binds a URL request to the network interface associated with the hotspot helper command instance.

func createTCPConnection(NWEndpoint) -> NWTCPConnection

Create a new TCP connection over the network associated with the command.

Deprecated

func createUDPSession(NWEndpoint) -> NWUDPSession

Creates a new UDP session over the network associated with the command.

Deprecated

### Response creation

func createResponse(NEHotspotHelperResult) -> NEHotspotHelperResponse

Create a response to the command.

enum NEHotspotHelperResult

### Instance Properties

var interface: NWInterface

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Commands

class NEHotspotHelperResponse

The hotspot helper’s response to a command.

class NEHotspotNetwork

Information about a Wi-Fi network associated with a command or a response.

