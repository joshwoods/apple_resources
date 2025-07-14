

- Device Management
- DeviceInformationResponse
- DeviceInformationResponse.QueryResponses
-  DeviceInformationResponse.QueryResponses.OSUpdateSettings 

Device Management Command

# DeviceInformationResponse.QueryResponses.OSUpdateSettings

The response dictionary that contains operating system update settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses.OSUpdateSettings
```

## Properties

`AutoCheckEnabled`

`boolean`

The preference to automatically check for app updates. This value is available in macOS 10.11 and later.

`AutomaticAppInstallationEnabled`

`boolean`

The preference to automatically install app updates. This value is available in macOS 10.11 and later.

`AutomaticOSInstallationEnabled`

`boolean`

The preference to automatically install operating system updates. This value is available in macOS 10.11 and later.

`AutomaticSecurityUpdatesEnabled`

`boolean`

The preference to automatically install system data files and security updates. This value is available in macOS 10.11 and later.

`BackgroundDownloadEnabled`

`boolean`

The preference to download app updates in the background. This value is available in macOS 10.11 and later.

`CatalogURL`

`string`

The URL to the software update catalog the client is using. This value is available in macOS 10.11 and later.

`IsDefaultCatalog`

`boolean`

If `true`, `CatalogURL` is the default catalog. This value is available in macOS 10.11 and later.

`PerformPeriodicCheck`

`boolean`

If `true`, start a new scan. This value is available in macOS 10.11 and later.

`PreviousScanDate`

`date`

The date of the last software update scan. This value is available in macOS 10.11 and later.

`PreviousScanResult`

`string`

Deprecated 

The result code of last software update scan; `"0"` = success. This value is available in macOS 10.11 and no longer availble in macOS 15 and later.

## See Also

### Commands

object DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

object DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem

The response dictionary that contains the administrator setup information.

object DeviceInformationResponse.QueryResponses.MDMOptions

The response dictionary that contains MDM options.

object DeviceInformationResponse.QueryResponses.OrganizationInfo

The response dictionary that contains organization information.

object DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty

The response dictionary that contains information about the active service subscription.

object DeviceInformationResponse.QueryResponses.SoftwareUpdateSettings

The response dictionary that contains information about the Software Update pane in Settings.

