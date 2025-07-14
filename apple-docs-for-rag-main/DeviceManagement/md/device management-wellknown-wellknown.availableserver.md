

- Device Management
- WellKnown
-  WellKnown.AvailableServer 

Object

# WellKnown.AvailableServer

The configuration details for an authentication server.

iOS 15.0+iPadOS 15.0+Device Assignment ServicesVPP License Management

``` source
object WellKnown.AvailableServer
```

## Properties

`BaseURL`

`string`

 (Required) 

The URL where the service resides. This is the base path for subsequent requests.

`Version`

`string`

 (Required) 

The server’s version string.

Possible Values: `mdm-byod, mdm-adde`

