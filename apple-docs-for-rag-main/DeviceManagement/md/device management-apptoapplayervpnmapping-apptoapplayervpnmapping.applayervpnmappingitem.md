

- Device Management
- AppToAppLayerVPNMapping
-  AppToAppLayerVPNMapping.AppLayerVPNMappingItem 

Device Management Profile

# AppToAppLayerVPNMapping.AppLayerVPNMappingItem

A dictionary defining a per-app VPN relationship.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object AppToAppLayerVPNMapping.AppLayerVPNMappingItem
```

## Properties

`DesignatedRequirement`

`string`

 (Required) 

The code signature designated requirement of the app using the per-app VPN.

`Identifier`

`string`

 (Required) 

The bundle identifier of the app using the per-app VPN.

`MatchTools`

`[`AppToAppLayerVPNMapping.AppLayerVPNMappingItem.MatchToolsItem`]`

An array of dictionaries. Each dictionary specifies a per-app VPN rule. Use this property to restrict this per-app VPN rule to only match the app’s spawned *helper tool* network traffic.

For example, to match network traffic that the `curl` command generates when run from the Terminal.app, create an app mapping payload for Terminal.app and set the payload’s `MatchTools` key to an array that contains a dictionary that matches the `curl` command-line tool.

If you don’t specify the `MatchTools` key, this per-app VPN rule matches all network traffic that the matching app and its spawned helper tools generate.

`Path`

`string`

The file-system path of the executable using the per-app VPN.

`SigningIdentifier`

`string`

 (Required) 

The code signature signing identifier of the app using the per-app VPN.

`VPNUUID`

`string`

 (Required) 

The identifier of the per-app VPN payload, which defines the per-app VPN that the app uses. See the `VPNUUID` key of the AppLayerVPN payload.

## Topics

### Profiles

object AppToAppLayerVPNMapping.AppLayerVPNMappingItem.MatchToolsItem

Specifies a per-app VPN rule to match network traffic that the app’s spawned command-line tool generates.

