

- ManagedSettings
- ManagedSettingsStore
-  siri 

Instance Property

# siri

Settings that affect Siri.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var siri: SiriSettings
```

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

struct SiriSettings

Constraints on the device’s Siri settings.

