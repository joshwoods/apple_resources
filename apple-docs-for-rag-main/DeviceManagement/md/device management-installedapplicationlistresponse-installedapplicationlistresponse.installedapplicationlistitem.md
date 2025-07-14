

- Device Management
- InstalledApplicationListResponse
-  InstalledApplicationListResponse.InstalledApplicationListItem 

Device Management Command

# InstalledApplicationListResponse.InstalledApplicationListItem

A dictionary that describes an app list item.

iOS 5.0+iPadOS 5.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstalledApplicationListResponse.InstalledApplicationListItem
```

## Properties

`AdHocCodeSigned`

`boolean`

If `true`, the app is ad-hoc code signed. This query is available in iOS 11.3 and later, and tvOS 11.3 and later.

`AppStoreVendable`

`boolean`

If `true`, the app came from the App Store and can participate in store features. For device-based Volume Purchase Program (VPP) apps, this value is `false`. This value is available in iOS 11.3 and later, and tvOS 11.3 and later.

`BetaApp`

`boolean`

If `true`, the app is part of the Apple Beta Software Program. This value is available in iOS 11.3 and later, and tvOS 11.3 and later.

`BundleSize`

`integer`

The app’s static bundle size, in bytes. This value is available in iOS 5 and later, and macOS 10.7 and later, and tvOS 10.2 and later.

`DeviceBasedVPP`

`boolean`

If `true`, installing the app didn’t require an Apple ID. This value is available in iOS 11.3 and later, and tvOS 11.3 and later.

`DistributorIdentifier`

`string`

The marketplace hosted application’s distributor ID. This value is available in iOS 17.4 and later.

`DownloadCancelled`

`boolean`

If `true`, the user canceled the download.

Default: `false`

`DownloadFailed`

`boolean`

If `true`, the download failed.

Default: `false`

`DownloadPaused`

`boolean`

If `true`, the user paused the download.

Default: `false`

`DownloadWaiting`

`boolean`

If `true`, the app is in the initial state, which is waiting to download.

Default: `false`

`DynamicSize`

`integer`

The size of the app’s file system in bytes, including the Documents, Library, and other directories. This value is available in iOS 5 and later, and tvOS 10.2 and later.

`ExternalVersionIdentifier`

`integer`

The app’s external version identifier, which you can use in the iTunes Search API to determine if an updated version of the app is available. Compare this value to the `externalId` value in the `contentMetadataLookupUrl` response from the `VPPServiceConfigSrv` endpoint. If these values don’t match, an updated version of the app may be available.

Note

A newer version of an app might not be available for installation on the device for a variety of reasons. A common reason is that the device’s operating system version or hardware is incompatible with the available version of the app.

`HasUpdateAvailable`

`boolean`

If `true`, the app has an update available. This key is present only for App Store apps. In macOS, this key is present only for Volume Purchase Program (VPP) apps. This status updates daily and isn’t always up-to-date when installing an app.

`Identifier`

`string`

The app’s identifier. This key is always be present on iOS and tvOS, but may be missing on macOS.

Note

For a watchOS app, the identifier is the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired.

`Installing`

`boolean`

If `true`, the app is downloading. If `false`, it’s already installed.

`IsAppClip`

`boolean`

If `true`, the app is an App Clip. Available in iOS 16 and later.

Default: `false`

`IsValidated`

`boolean`

If `true`, the app is valid and can run on the device. If the app is enterprise-distributed and unvalidated, it won’t be able to run until validation has occurred. This value is available in iOS 9.2 and later, and tvOS 10.2 and later.

`Name`

`string`

The app’s name.

`ShortVersion`

`string`

The app’s short version.

`Source`

`string`

The source of the application. When the app is managed by Declarative Device Management this value is `Declarative Device Management`.

`Version`

`string`

The app’s version.

## See Also

### Commands

object InstalledApplicationListResponse.ErrorChainItem

A dictionary that describes an error chain item.

