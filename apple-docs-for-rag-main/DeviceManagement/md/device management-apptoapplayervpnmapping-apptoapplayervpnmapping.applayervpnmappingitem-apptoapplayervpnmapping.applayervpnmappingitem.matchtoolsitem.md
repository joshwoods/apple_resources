

- Device Management
- AppToAppLayerVPNMapping
- AppToAppLayerVPNMapping.AppLayerVPNMappingItem
-  AppToAppLayerVPNMapping.AppLayerVPNMappingItem.MatchToolsItem 

Device Management Profile

# AppToAppLayerVPNMapping.AppLayerVPNMappingItem.MatchToolsItem

Specifies a per-app VPN rule to match network traffic that the app’s spawned command-line tool generates.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object AppToAppLayerVPNMapping.AppLayerVPNMappingItem.MatchToolsItem
```

## Properties

`DesignatedRequirement`

`string`

 (Required) 

The code signature designated requirement of the command-line tool using the per-app VPN.

`Path`

`string`

The file-system path of the command-line tool using the per-app VPN.

`SigningIdentifier`

`string`

 (Required) 

The code signature signing identifier of the command-line tool using the per-app VPN.

