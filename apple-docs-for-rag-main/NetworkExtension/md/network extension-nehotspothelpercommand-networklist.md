

- Network Extension
- NEHotspotHelperCommand
-  networkList 

Instance Property

# networkList

The list of networks associated with the command.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var networkList: [NEHotspotNetwork]? { get }
```

## Discussion

This property will be nil unless `commandType` is `kNEHotspotHelperCommandTypeFilterScanList`.

## See Also

### Command information

var commandType: NEHotspotHelperCommandType

The type of the command

enum NEHotspotHelperCommandType

var network: NEHotspotNetwork?

The network associated with the command.

