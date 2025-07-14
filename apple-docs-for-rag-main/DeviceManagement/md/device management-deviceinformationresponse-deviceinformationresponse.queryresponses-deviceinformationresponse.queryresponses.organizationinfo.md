

- Device Management
- DeviceInformationResponse
- DeviceInformationResponse.QueryResponses
-  DeviceInformationResponse.QueryResponses.OrganizationInfo 

Device Management Command

# DeviceInformationResponse.QueryResponses.OrganizationInfo

The response dictionary that contains organization information.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses.OrganizationInfo
```

## Properties

`OrganizationAddress`

`string`

The organization’s address. Use the LF character (`&#10`) to insert line breaks. This value is available in iOS 7 and later, macOS 10.11 and later, and tvOS 9 and later.

`OrganizationEmail`

`string`

The orgnization’s support email address. This value is available in iOS 7 and later, macOS 10.11 and later, and tvOS 9 and later.

`OrganizationMagic`

`string`

A unique identifier for the various services a single organization manages. This value is available in iOS 7 and later, macOS 10.11 and later, and tvOS 9 and later.

`OrganizationName`

`string`

 (Required) 

A string that describes the organization operating the MDM server. This value is available in iOS 7 and later, macOS 10.11 and later, and tvOS 9 and later.

`OrganizationPhone`

`string`

The organization’s phone number. This value is available in iOS 7 and later, macOS 10.11 and later, and tvOS 9 and later.

## See Also

### Commands

object DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

object DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem

The response dictionary that contains the administrator setup information.

object DeviceInformationResponse.QueryResponses.MDMOptions

The response dictionary that contains MDM options.

object DeviceInformationResponse.QueryResponses.OSUpdateSettings

The response dictionary that contains operating system update settings.

object DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty

The response dictionary that contains information about the active service subscription.

object DeviceInformationResponse.QueryResponses.SoftwareUpdateSettings

The response dictionary that contains information about the Software Update pane in Settings.

