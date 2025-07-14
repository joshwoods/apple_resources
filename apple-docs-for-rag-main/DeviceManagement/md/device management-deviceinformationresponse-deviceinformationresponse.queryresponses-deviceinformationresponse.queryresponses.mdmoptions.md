

- Device Management
- DeviceInformationResponse
- DeviceInformationResponse.QueryResponses
-  DeviceInformationResponse.QueryResponses.MDMOptions 

Device Management Command

# DeviceInformationResponse.QueryResponses.MDMOptions

The response dictionary that contains MDM options.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses.MDMOptions
```

## Properties

`ActivationLockAllowedWhileSupervised`

`boolean`

If `true`, a supervised device registers itself with Activation Lock when the user enables Find My. Unsupervised devices ignore this value. This value is available in iOS 7 and later, macOS 11 and later, and tvOS 9 and later.

Default: `false`

`BootstrapTokenAllowed`

`boolean`

If `true`, the server supports Bootstrap Token commands. This value is available in macOS 11 and later.

Default: `false`

`PromptUserToAllowBootstrapTokenForAuthentication`

`boolean`

If `true`, the device can accept a Bootstrap Token from the MDM server instead of prompting for user authentication prior to installation. This only applies when `BootstrapTokenAllowedForAuthentication` is `true` in the SecurityInfoResponse.SecurityInfo response. This value is available for Apple silicon devices in macOS 11 and later.

Default: `false`

## See Also

### Commands

object DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

object DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem

The response dictionary that contains the administrator setup information.

object DeviceInformationResponse.QueryResponses.OrganizationInfo

The response dictionary that contains organization information.

object DeviceInformationResponse.QueryResponses.OSUpdateSettings

The response dictionary that contains operating system update settings.

object DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty

The response dictionary that contains information about the active service subscription.

object DeviceInformationResponse.QueryResponses.SoftwareUpdateSettings

The response dictionary that contains information about the Software Update pane in Settings.

