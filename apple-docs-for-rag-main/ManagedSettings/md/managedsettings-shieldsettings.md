

- ManagedSettings
-  ShieldSettings 

Structure

# ShieldSettings

Constraints that indicate what apps and websites to cover with a shielding view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct ShieldSettings
```

## Topics

### Blocking Apps and Websites

var applications: Set&lt;ApplicationToken>?

Applications for the system to cover with a shielding view.

static let applications: SettingMetadata&lt;Set&lt;ApplicationToken>>

The metadata for the configuration that specifies apps for the system to cover with a shielding view.

var webDomains: Set&lt;WebDomainToken>?

Websites for the system to cover with a shielding view.

static let webDomains: SettingMetadata&lt;Set&lt;WebDomainToken>>

The metadata for the configuration that specifies websites for the system to shield.

### Blocking Categories of Apps and Websites

enum ActivityCategoryPolicy

Policies available for shielding activities based on their category.

var applicationCategories: ShieldSettings.ActivityCategoryPolicy&lt;Application>?

Categories of apps for the system to cover with a shielding view.

static let applicationCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;Application>>

The metadata for the configuration that specifies categories of apps for the system to cover with a shielding view.

var webDomainCategories: ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>?

Categories of websites for the system to cover with a shielding view.

static let webDomainCategories: SettingMetadata&lt;ShieldSettings.ActivityCategoryPolicy&lt;WebDomain>>

The metadata for the configuration that specifies categories of websites for the system to shield.

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

var siri: SiriSettings

Settings that affect Siri.

struct SiriSettings

Constraints on the device’s Siri settings.

