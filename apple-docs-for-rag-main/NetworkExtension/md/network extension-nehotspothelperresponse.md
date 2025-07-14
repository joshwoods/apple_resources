

- Network Extension
-  NEHotspotHelperResponse 

Class

# NEHotspotHelperResponse

The hotspot helper’s response to a command.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class NEHotspotHelperResponse
```

## Topics

### Response properties

func setNetwork(NEHotspotNetwork)

Set the network that conveys the confidence level.

func setNetworkList([NEHotspotNetwork])

Set the list of handled networks.

### Response celivery

func deliver()

Deliver the response to the system.

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

class NEHotspotHelperCommand

A command for the hotspot helper to handle.

class NEHotspotNetwork

Information about a Wi-Fi network associated with a command or a response.

