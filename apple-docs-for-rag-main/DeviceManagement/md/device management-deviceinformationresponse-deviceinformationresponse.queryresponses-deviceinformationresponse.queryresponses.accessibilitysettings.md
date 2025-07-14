

- Device Management
- DeviceInformationResponse
- DeviceInformationResponse.QueryResponses
-  DeviceInformationResponse.QueryResponses.AccessibilitySettings 

Device Management Command

# DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses.AccessibilitySettings
```

## Properties

`BoldTextEnabled`

`boolean`

If `true`, the device has enabled bold text.

`GrayscaleEnabled`

`boolean`

If `true`, the device has enabled grayscale display.

`IncreaseContrastEnabled`

`boolean`

If `true`, the device has enabled increase contrast.

`ReduceMotionEnabled`

`boolean`

If `true`, the device has enabled reduced motion.

`ReduceTransparencyEnabled`

`boolean`

If `true`, the device has enabled reduced transparency.

`TextSize`

`integer`

The accessibility text size apps that support dynamic text use. 0 is the smallest value, and 11 is the largest available.

`-1` indicates that the current size is unknown or hasn’t been explicitly set.

Possible Values: `-1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11`

`TouchAccommodationsEnabled`

`boolean`

If `true`, the device has enabled touch accommodations.

`VoiceOverEnabled`

`boolean`

If `true`, the device has enabled voiceover.

`ZoomEnabled`

`boolean`

If `true`, the device has enabled zoom.

## See Also

### Commands

object DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem

The response dictionary that contains the administrator setup information.

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

