

- Device Management
- SecurityInfoResponse
- SecurityInfoResponse.SecurityInfo
- SecurityInfoResponse.SecurityInfo.FirewallSettings
-  SecurityInfoResponse.SecurityInfo.FirewallSettings.ApplicationsItem 

Device Management Command

# SecurityInfoResponse.SecurityInfo.FirewallSettings.ApplicationsItem

A dictionary that describes the allowed apps.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SecurityInfoResponse.SecurityInfo.FirewallSettings.ApplicationsItem
```

## Properties

`Allowed`

`boolean`

If `true`, the app is an allowed app.

`BundleID`

`string`

The app’s bundle identifier.

`Name`

`string`

The app’s display name if it’s determinable from the `BundleID`.

## Discussion

This dictionary is available in macOS 10.12 and later.

