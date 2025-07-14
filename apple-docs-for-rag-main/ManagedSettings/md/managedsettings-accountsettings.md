

- ManagedSettings
-  AccountSettings 

Structure

# AccountSettings

An object that configures whether a user can modify their device’s account settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct AccountSettings
```

## Topics

### Constraining Accounts

var lockAccounts: Bool?

A Boolean value that indicates whether to prevent the user from changing their account information.

static let lockAccounts: SettingMetadata&lt;Bool>

A description of the setting that controls whether a user can modify their account information.

## Relationships

### Conforms To

- ManagedSettingsGroup

## See Also

### Restricting Device Settings

var account: AccountSettings

Settings that affect accounts.

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

struct SiriSettings

Constraints on the device’s Siri settings.

