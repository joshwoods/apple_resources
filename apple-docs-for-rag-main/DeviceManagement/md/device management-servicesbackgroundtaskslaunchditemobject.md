

- Device Management
-  ServicesBackgroundTasksLaunchdItemObject 

Object

# ServicesBackgroundTasksLaunchdItemObject

A dictionary of launchd configurations.

macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object ServicesBackgroundTasksLaunchdItemObject
```

## Properties

`Context`

`string`

 (Required) 

Indicates whether the launchd configuration file is applied to the system daemon, or system agent domain.

Possible Values: `daemon, agent`

`FileAssetReference`

`string`

 (Required) 

Specifies the identifier of an asset declaration containing a reference to the launchd configuration file for the background task. The referenced data must be a property list file conforming to the launchd.plist format. The asset’s “ContentType” and “Hash-SHA-256” keys in the “Reference” key are required.

