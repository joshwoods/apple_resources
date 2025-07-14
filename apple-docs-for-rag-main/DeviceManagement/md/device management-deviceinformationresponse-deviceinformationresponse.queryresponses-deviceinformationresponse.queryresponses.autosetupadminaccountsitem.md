

- Device Management
- DeviceInformationResponse
- DeviceInformationResponse.QueryResponses
-  DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem 

Device Management Command

# DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem

The response dictionary that contains the administrator setup information.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem
```

## Properties

`GUID`

`string`

The `GeneratedUID` of the administrator account. This value is available in macOS 10.11 and later.

`shortName`

`string`

The short name of the administrator account. This value is available in macOS 10.11 and later.

## See Also

### Commands

object DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

object DeviceInformationResponse.QueryResponses.MDMOptions

The response dictionary that contains MDM options.

object DeviceInformationResponse.QueryResponses.OrganizationInfo

The response dictionary that contains organization information.

object DeviceInformationResponse.QueryResponses.OSUpdateSettings

The response dictionary that contains operating system update settings.

object DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty

The response dictionary that contains information about the active service subscription.

object DeviceInformationResponse.QueryResponses.SoftwareUpdateSettings

The response dictionary that contains information about the Software Update pane in Settings.

