

- Device Management
-  StatusAppManagedListAppObject 

Object

# StatusAppManagedListAppObject

A dictionary that describes a declarative managed app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object StatusAppManagedListAppObject
```

## Properties

`_removed`

`boolean`

If `true`, the system removed the app and only this key and the `identifier` key are present in the status item object.

Default: `false`

`config-state`

StatusAppManagedListManagedConfigurationObject

The status of app or extension managed configurations. This key is only present when managed configurations are available for the managed app or any of its extensions.

`declaration-identifier`

`string`

The identifier of the declaration that controls the app.

`external-version-id`

`integer`

The app’s external version ID. You can also retrieve this value from the store through the contentMetadataLookupUrl of VPPServiceConfigSrv.

In the response from `uclient-api.itunes.apple.com` URL, there’s an `externalId` at the path `results..offers[0].version.externalId`. If the current external version identifier of an app on the store doesn’t match the external version identifier reported by the device, there may be an app update available for the device.

`identifier`

`string`

 (Required) 

The app’s bundle id, which is unique.

`name`

`string`

The name of the app.

`reasons`

`[`StatusAppManagedListStatusReasonObject`]`

An array that contains additional details about the app state, including errors.

`short-version`

`string`

The short version of the app.

`state`

`string`

The status of the app, which has the following possible values:

`optional`  
The app is optional and the user has to trigger its installation.

`queued`  
Installation of the app started.

`prompting-for-consent`  
The system is displaying a prompt to the user to proceed with app installation.

`prompting-for-login`  
The system is displaying an App Store sign-in prompt to the user to allow app installation.

`prompting-for-management`  
The system is displaying a prompt to the user to allow changing the installed app to a managed app.

`downloading`  
The system is downloading an app update.

`installing`  
The system is installing an app update.

`managed`  
The app is installed and managed.

`managed-but-uninstalled`  
The app is managed, but the user removed it. The app remains managed if the system installs it again.

`failed`  
An app update failed.

Possible Values: `optional, queued, prompting-for-consent, prompting-for-login, prompting-for-management, downloading, installing, managed, managed-but-uninstalled, failed`

`update-state`

`string`

The update status of the app, which has the following possible values:

`available`  
An update is available for the app.

`prompting-for-update`  
The system is displaying a prompt to the user to proceed with app installation.

`prompting-for-update-login`  
The system is displaying an App Store sign-in prompt to the user to allow app installation.

`updating`  
The app is updating.

`failed`  
The app update failed.

Note

This key is only present if `state` is `managed` and an update is available.

Possible Values: `available, prompting-for-update, prompting-for-update-login, updating, failed`

`version`

`string`

The version of the app.

## Topics

### Objects

object StatusAppManagedListStatusReasonObject

A dictionary that contains details about a declarative managed app’s state.

object StatusAppManagedListManagedConfigurationObject

A dictionary that contains details about a declarative managed app’s managed configuration.

