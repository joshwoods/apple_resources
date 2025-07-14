

- Device Management
- DeviceInformationResponse
-  DeviceInformationResponse.QueryResponses 

Device Management Command

# DeviceInformationResponse.QueryResponses

The response dictionary that contains information about the device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeviceInformationResponse.QueryResponses
```

## Properties

`AccessibilitySettings`

DeviceInformationResponse.QueryResponses.AccessibilitySettings

The current state of settable accessibility settings. Available in iOS 16 and later.

`ActiveManagedUsers`

`[string]`

An array of the directory GUIDs of the logged-in managed users. If one of these users is currently logged in to the console, the `CurrentConsoleManagedUser` key returns the GUID of that user. Requires the Device Information access right. Available in macOS 10.11 and later.

`AppAnalyticsEnabled`

`boolean`

If `true`, the device is sharing app analytics. Requires the Device Information access right. Available in iOS 9.3 and later.

`AutoSetupAdminAccounts`

`[`DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem`]`

The contents of DeviceInformationResponse.QueryResponses.AutoSetupAdminAccountsItem, which Setup Assistant automatically created during DEP enrollment. Requires the Device Information access right. Available in macOS 10.11 and later.

`AvailableDeviceCapacity`

`number`

The available capacity in floating-point base-10 gigabytes (GB) on iOS and macOS 12 or later. The capacity is in base-2 gibibytes (GiB) on macOS 11 and earlier. Requires the Device Information access right. Available in iOS 4 and later, and macOS 10.7 and later.

`AwaitingConfiguration`

`boolean`

If `true` on the device channel, the device is still waiting for a DeviceConfiguredCommand to continue through Setup Assistant.

If `true` on the user channel (Shared iPad only), the device is still waiting for a UserConfiguredCommand to continue through Setup Assistant and finish login.

`BatteryLevel`

`number`

The battery level, between `0.0` and `1.0`, or `-1.0` if MDM can’t determine the battery level. Requires the Device Information access right. Available in iOS 5 and later, and macOS 13.3 and later.

`BluetoothMAC`

`string`

The Bluetooth media access control (MAC) address. Requires the Network Information access right.

`BuildVersion`

`string`

The operating system version. Requires the Device Information access right.

`CellularTechnology`

`integer`

The cellular technology type, which is one of the following values:

- `0`: None

- `1`: GSM

- `2`: CDMA

- `3`: GSM and CDMA

Requires the Device Information access right. Available in iOS 4.2.6 and later.

Possible Values: `0, 1, 2, 3`

`DataRoamingEnabled`

`boolean`

If `true`, the device has enabled data roaming. Requires the Network Information access right. Available in iOS 5 and later.

`DeviceCapacity`

`number`

The total capacity in floating-point base-10 gigabytes (GB) on iOS and macOS 12 or later. The capacity is in base-2 gibibytes (GiB) on macOS 11 and earlier. Requires the Device Information access right. Available in iOS 4 and later, and macOS 10.7 and later.

`DeviceID`

`string`

The device identifier. Requires the Device Information access right. Available in tvOS 6 and later.

`DeviceName`

`string`

The device name. Requires the Device Information access right.

`DevicePropertiesAttestation`

`[data]`

The key to get an attestation of the device’s properties. Available in iOS 16 and later, macOS 14 and later, tvOS 16 and later, and watchOS 10 and later.

`DiagnosticSubmissionEnabled`

`boolean`

If `true`, the device has enabled diagnostic submission. Requires the Device Information access right. Available in iOS 9.3 and later.

`EACSPreflight`

`string`

Specifies whether the device can perform an EraseDeviceCommand using Erase All Content and Settings (EACS), which is one of the following values:

`success`  
The device supports EACS.

`not supported`  
The device is too old to support EACS.

`unknown failure`  
A problem occurred for which there isn’t a more specific error message.

`(other string)`  
A reason why the device can’t perform EACS, such as “System is not sealed”

`EASDeviceIdentifier`

`string`

The device identifier for Exchange Active Sync (EAS). Requires the Device Information access right. Available in iOS 7 and later.

`EstimatedResidentUsers`

`integer`

The estimated number of users that can use this shared iPad device, according to the space available on the device and each user’s quota. Requires the Device Information access right. Available in iOS 14 and later.

`EthernetMAC`

`string`

The primary Ethernet MAC address. Requires the Network Information access right. Available in macOS 10.7 and later.

`HasBattery`

`boolean`

If `true`, the device has an internal battery.

`HostName`

`string`

The host name. Available in macOS 10.11 and later.

`IsActivationLockSupported`

`boolean`

If `true`, the device supports Activation Lock. Also see `IsActivationLockManageable` in SecurityInfoResponse.SecurityInfo.ManagementStatus. Available in macOS 10.9 and later.

`IsAppleSilicon`

`boolean`

If `true`, the macOS device uses an Apple silicon chip.

`IsCloudBackupEnabled`

`boolean`

If `true`, the device has enabled iCloud backup. Requires the Device Information access right. Available in iOS 7.1 and later.

`IsDeviceLocatorServiceEnabled`

`boolean`

If `true`, the device has enabled a device locator service, such as Find My. Requires the Device Information access right. Available in iOS 7 and later.

`IsDoNotDisturbInEffect`

`boolean`

If `true`, the device is in Do Not Disturb (DND) mode. This value is `true` even if DND is only in effect for a locked device. Requires the Device Information access right. Available in iOS 7 and later.

`IsMDMLostModeEnabled`

`boolean`

If `true`, the device has enabled Managed Lost Mode. Requires the Device Information access right. Available in iOS 9.3 and later.

`IsMultiUser`

`boolean`

If `true`, the device is in ephemeral multiuser mode. Requires the Device Information access right. Available in iOS 9.3 and later.

`IsNetworkTethered`

`boolean`

If `true`, the device is network-tethered. Requires the Network Information access right. Available in iOS 10.3 and later.

`IsSupervised`

`boolean`

If `true`, it’s a supervised device. Requires the Device Information access right. Available in iOS 6 and later, macOS 10.15 and later, and tvOS 9 and later.

`iTunesStoreAccountHash`

`string`

A hash of the logged-in iTunes Store account. Also see GetVppUserRequest. Requires the App Installation access right.

`iTunesStoreAccountIsActive`

`boolean`

If `true`, the device has an active iTunes Store account. Requires the App Installation access right.

`LastCloudBackupDate`

`date`

The date of the last iCloud backup. Available in iOS 8 and later.

`LocalHostName`

`string`

The local host name from Bonjour. Available in macOS 10.11 and later.

`MaximumResidentUsers`

`integer`

The maximum number of users that can use this shared iPad device. Starting with iOS 13.4, the value that returns is always `32`. Requires the Device Information access right. Available in iOS 9.3 and later.

`MDMOptions`

DeviceInformationResponse.QueryResponses.MDMOptions

The contents of SettingsCommand.Command.Settings.MDMOptions.MDMOptions.

`Model`

`string`

The model. Requires the Device Information access right.

`ManagedAppleIDDefaultDomains`

`[string]`

The list of domains that the device suggests on the Shared iPad login screen. Available in iOS 16 and later.

`ModelName`

`string`

The model name, such as *iPhone*. Requires the Device Information access right.

`ModemFirmwareVersion`

`string`

The modem firmware version. Requires the Device Information access right. Available in iOS 4.0 and later.

`ModelNumber`

`string`

The device’s hardware model number including region info, for example, `MK1A3LL/A`. Requires the Device Information access right. Requires Apple silicon on macOS.

`OnlineAuthenticationGracePeriod`

`integer`

The grace period for Shared iPad online authentication (in days). A value of `0` indicates that the device requires online authentication for every login. Available in iOS 16 and later.

`OrganizationInfo`

DeviceInformationResponse.QueryResponses.OrganizationInfo

The contents of SettingsCommand.Command.Settings.OrganizationInfo.OrganizationInfo.

`OSUpdateSettings`

DeviceInformationResponse.QueryResponses.OSUpdateSettings

The contents of DeviceInformationResponse.QueryResponses.OSUpdateSettings. Requires the Device Information access right. Available in macOS 10.11 and later.

`OSVersion`

`string`

The operating system version. Requires the Device Information access right.

`PersonalHotspotEnabled`

`boolean`

If `true,` the device has enabled Personal Hotspot, which isn’t available for all carriers. Requires the Network Information access right. Available in iOS 7.0 and later.

`PINRequiredForDeviceLock`

`boolean`

If `true`, the DeviceLockCommand requires a PIN. Available in macOS 11 and later.

`PINRequiredForEraseDevice`

`boolean`

If `true`, the EraseDeviceCommand requires a PIN. Available in macOS 11 and later.

`ProductName`

`string`

The product name, such as *iPad8,12*. Requires the Device Information access right.

`ProvisioningUDID`

`string`

The device identifier used in provisioning profiles. This value differs from the UDID on Macs with Apple silicon. Available in macOS 11.3 and later.

`PushToken`

`data`

The push token for the user-channel connection, in the same format as in TokenUpdateRequest. MDM ignores this query for the device channel. Requires the Device Information access right. Available in iOS 9.3 and later, and macOS 10.12 and later.

`QuotaSize`

`integer`

The quota size in megabytes for each user on this shared iPad device. Requires the Device Information access right. Available in iOS 13.4 and later.

`ResidentUsers`

`integer`

The number of users currently on this shared iPad device. Requires the Device Information access right. Available in iOS 13.4 and later.

`SerialNumber`

`string`

The serial number. Requires the Device Information access right.

`ServiceSubscriptions`

`[`DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty`]`

The contents of DeviceInformationResponse.QueryResponses.ServiceSubscriptionProperty. Requires the Network Information access right.

`SkipLanguageAndLocaleSetupForNewUsers`

`boolean`

If `true`, skip the language and country/region panes for new users on Shared iPad.

`SoftwareUpdateDeviceID`

`string`

The device identifier that you use to look up available OS updates through https://gdmf.apple.com/v2/pmv. Available in iOS 15 and later, and macOS 12 and later.

`SoftwareUpdateSettings`

DeviceInformationResponse.QueryResponses.SoftwareUpdateSettings

The device settings that control which updates appear in the Software Update pane in Settings. Available in iOS 14.5 and later.

`SupplementalBuildVersion`

`string`

The supplemental OS build version.

`SupplementalOSVersionExtra`

`string`

The OS update rapid security response version letter.

`SupportsiOSAppInstalls`

`boolean`

If `true`, the device supports iOS/iPadOS app installs through MDM. Available in macOS 11 and later.

`SupportsLOMDevice`

`boolean`

If `true`, the device can receive `PowerON`, `PowerOFF`, and `Reset` commands from a lights-out management (LOM) controller. Available in macOS 11 and later.

`SystemIntegrityProtectionEnabled`

`boolean`

If `true`, the device has enabled System Integrity Protection. Requires the Device Information access right. Available in macOS 10.12 and later.

`TemporarySessionOnly`

`boolean`

If `true`, the device only allows temporary sessions.

`TemporarySessionTimeout`

`integer`

The timeout interval for the temporary session. A value of `0` indicates that there’s no timeout.

`TimeZone`

`string`

The current Internet Assigned Numbers Authority (IANA) time zone database name. Requires the Device Information access right. Available in iOS 14 and later, and tvOS 14 and later.

`UDID`

`string`

The unique identifier of the device.

`UserSessionTimeout`

`integer`

The timeout interval for the user session. A value of `0` indicates that there’s no timeout.

`WiFiMAC`

`string`

The Wi-Fi MAC address. Requires the Network Information access right.

`CurrentCarrierNetwork`

`string`

Deprecated 

The name of the current carrier network. Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`CarrierSettingsVersion`

`string`

Deprecated 

The version of the carrier settings. Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`CurrentMCC`

`string`

Deprecated 

The current mobile country code (MCC). Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`CurrentMNC`

`string`

Deprecated 

The current mobile network code (MNC). Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`ICCID`

`string`

Deprecated 

The integrated circuit card (ICC) identifier for the installed SIM card. Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`IMEI`

`string`

Deprecated 

The International Mobile Equipment Identity (IMEI) number. Requires the Device Information access right. Available as of iOS 4 and deprecated in iOS 16.

`IsActivationLockEnabled`

`boolean`

Deprecated 

If `true`, the device has enabled Activation Lock. Requires the Device Information access right. Available as of iOS 7 and macOS 10.9, and deprecated in iOS 16 and macOS 13.

`IsRoaming`

`boolean`

Deprecated 

If `true`, the device is roaming. Requires the Network Information access right. IAvailable as of iOS 4.2 and deprecated in iOS 16.

`MEID`

`string`

Deprecated 

The mobile equipment identifier (MEID) number. Requires the Device Information access right. Available as of iOS 4 and deprecated in iOS 16.

`PhoneNumber`

`string`

Deprecated 

The raw phone number without punctuation and including the country code. Requires the Network Information access right. Available as of iOS 4 and deprecated in iOS 16.

`SIMCarrierNetwork`

`string`

Deprecated 

Apple no longer supports this query. Use `SubscriberCarrierNetwork` instead.

`SIMMCC`

`string`

Deprecated 

Apple no longer supports this query. Use `SubscriberMCC` instead.

`SIMMNC`

`string`

Deprecated 

Apple no longer supports this query. Use `SubscriberMNC` instead.

`SubscriberCarrierNetwork`

`string`

Deprecated 

The name of the home carrier network. Requires the Network Information access right. Available as of iOS 5 and deprecated in iOS 16.

`SubscriberMCC`

`string`

Deprecated 

The home Mobile Country Code (MCC). Requires the Network Information access right. Available as of iOS 4.2.6 and deprecated in iOS 16.

`SubscriberMNC`

`string`

Deprecated 

The key to get the home Mobile Network Code (MNC). Requires the Network Information access right. Available as of iOS 4.2.6 and deprecated in iOS 16.

`VoiceRoamingEnabled`

`boolean`

Deprecated 

If `true`, the device has enabled voice roaming, which isn’t available for all carriers. Requires the Network Information access right. Requires the Device Information access right. Available as of iOS 5 and deprecated in iOS 16.

## Topics

### Commands

object DeviceInformationResponse.QueryResponses.AccessibilitySettings

The response dictionary that contains the devices accessibility settings.

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

## See Also

### Commands

object DeviceInformationResponse.ErrorChainItem

A dictionary that describes an error chain.

