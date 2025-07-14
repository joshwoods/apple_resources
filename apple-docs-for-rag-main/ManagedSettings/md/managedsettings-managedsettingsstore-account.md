

- ManagedSettings
- ManagedSettingsStore
-  account 

Instance Property

# account

Settings that affect accounts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var account: AccountSettings
```

## See Also

### Restricting Device Settings

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

struct SiriSettings

Constraints on the device’s Siri settings.

