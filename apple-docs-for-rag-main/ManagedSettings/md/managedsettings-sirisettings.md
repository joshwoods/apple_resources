

- ManagedSettings
-  SiriSettings 

Structure

# SiriSettings

Constraints on the device’s Siri settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct SiriSettings
```

## Topics

### Restricting Siri Usage

var denySiri: Bool?

A Boolean value that indicates whether to prevent access to Siri.

static let denySiri: SettingMetadata&lt;Bool>

The metadata for the constraint that configures access to Siri.

## Relationships

### Conforms To

- ManagedSettingsGroup

## See Also

### Restricting Device Settings

var account: AccountSettings

Settings that affect accounts.

struct AccountSettings

An object that configures whether a user can modify their device’s account settings.

var cellular: CellularSettings

Settings that affect cellular networking.

struct CellularSettings

Constraints on the user’s cellular networking settings.

var dateAndTime: DateAndTimeSettings

Settings that affect the date and time.

struct DateAndTimeSettings

Constraints on the device’s date and time settings.

var passcode: PasscodeSettings

Settings that affect the device passcode.

struct PasscodeSettings

Constraints on a user’s ability to change their device’s passcode.

var shield: ShieldSettings

Settings that affect what activities the system covers with a shielding view on this device.

struct ShieldSettings

Constraints that indicate what apps and websites to cover with a shielding view.

var siri: SiriSettings

Settings that affect Siri.

