

- Device Management
-  StatusSoftwareUpdateInstallReasonDictionaryObject 

Object

# StatusSoftwareUpdateInstallReasonDictionaryObject

A status report that contains details about the reason for a pending software update.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 18.4+Device Assignment ServicesVPP License Management

``` source
object StatusSoftwareUpdateInstallReasonDictionaryObject
```

## Properties

`declaration-id`

`string`

The identifier of the declaration that caused the software update to occur. This key is present only if the `reason` array contains the `declaration` value.

`reason`

`[string]`

 (Required) 

A list of reasons for the pending software update. An empty list indicates that no software update is pending.

Possible Values: `system-settings, install-tonight, auto-update, notification, setup-assistant, command-line, mdm, declaration`

