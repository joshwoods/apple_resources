

- Device Management
- APN
- APN.DefaultsData
-  APN.DefaultsData.ApnsItem 

Device Management Profile

# APN.DefaultsData.ApnsItem

A dictionary that describes an APN configuration.

iOS 4.0–7.0DeprecatediPadOS 4.0–7.0DeprecatedDevice Assignment ServicesVPP License Management

``` source
object APN.DefaultsData.ApnsItem
```

## Properties

`apn`

`string`

Deprecated   (Required) 

The access point name.

`password`

`data`

Deprecated 

The password for the user. For obfuscation purposes, the system encodes the password. If missing, the device prompts for the password during profile installation.

`proxy`

`string`

Deprecated 

The IP address or URL of the APN proxy.

`proxyPort`

`integer`

Deprecated 

The port number of the APN proxy.

`username`

`string`

Deprecated 

The user name. If missing, the device prompts for it during profile installation.

