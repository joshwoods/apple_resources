

- Device Management
-  StatusMDMAppAppObject 

Object

# StatusMDMAppAppObject

A status report that contains details about an MDM-installed app.

iOS 16.0+iPadOS 16.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object StatusMDMAppAppObject
```

## Properties

`_removed`

`boolean`

If `true`, the system removed the app and only this key and the `identifier` key are present in the status item object.

Default: `false`

`external-version-id`

`string`

The application’s external version ID. Use Service Config to get the `contentMetadataLookupUrl` endpoint. In the response from that URL, find a key named `externalId` at the path `results..offers[0].version.externalId`. If the current external version identifier of an app on the store doesn’t match the external version identifier reported by the device, there may be an app update available for the device.

`identifier`

`string`

 (Required) 

The app’s bundle id, which is unique.

`name`

`string`

The name of the app.

`short-version`

`string`

The short version of the app.

`state`

`string`

The status of the app that ManagedApplicationListCommand reports.

Possible Values: `queued, needs-redemption, redeeming, prompting, prompting-for-login, validating-purchase, prompting-for-update, prompting-for-update-login, prompting-for-management, validating-update, updating, installing, managed, managed-but-uninstalled, unknown, user-installed-app, user-rejected, update-rejected, management-rejected, failed`

`version`

`string`

The version of the app.

