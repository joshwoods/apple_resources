

- ManagedSettings
-  CellularSettings 

Structure

# CellularSettings

Constraints on the user’s cellular networking settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct CellularSettings
```

## Overview

Use `CellularSettings` to constrain the user’s ability to modify cellular settings in the Settings app.

## Topics

### Locking App Access to Cell Data

var lockAppCellularData: Bool?

A Boolean value that indicates whether to prevent the user from changing cellular data settings.

static let lockAppCellularData: SettingMetadata&lt;Bool>

The metadata associated with the constraint that locks the cellular data setting.

### Locking the Device’s Cell Plan

var lockCellularPlan: Bool?

A Boolean value that indicates whether to prevent the user from changing their cellular plan.

static let lockCellularPlan: SettingMetadata&lt;Bool>

The metadata associated with the constraint that locks the user’s cellular plan.

### Locking the Device’s eSIM Settings

var lockESIM: Bool?

A Boolean value that indicates whether to prevent the user from changing their eSIM settings.

static let lockESIM: SettingMetadata&lt;Bool>

The metadata associated with the constraint that locks the user’s eSIM settings.

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

