

- Network Extension
-  NEHotspotHelperCommandType 

Enumeration

# NEHotspotHelperCommandType

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum NEHotspotHelperCommandType
```

## Topics

### Command Types

case none

Placeholder for the null command.

case filterScanList

Filter the Wi-Fi scan list.

case evaluate

Evaluate the network.

case authenticate

Authenticate to the network.

case presentUI

Present user interface.

case maintain

Maintain the connection to the network.

case logoff

Logoff the network.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Command information

var commandType: NEHotspotHelperCommandType

The type of the command

var network: NEHotspotNetwork?

The network associated with the command.

var networkList: [NEHotspotNetwork]?

The list of networks associated with the command.

