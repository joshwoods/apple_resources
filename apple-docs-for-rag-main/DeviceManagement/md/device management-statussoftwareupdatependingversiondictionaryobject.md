

- Device Management
-  StatusSoftwareUpdatePendingVersionDictionaryObject 

Object

# StatusSoftwareUpdatePendingVersionDictionaryObject

A dictionary that contains details about a pending software update.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object StatusSoftwareUpdatePendingVersionDictionaryObject
```

## Properties

`build-version`

`string`

 (Required) 

The build version of the pending software update, including any rapid security response version. This string is empty if no update is pending.

`os-version`

`string`

 (Required) 

The OS version of the pending software update, including any rapid security response version. This string is empty if no update is pending.

`target-local-date-time`

`string`

