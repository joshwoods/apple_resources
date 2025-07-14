

- Device Management
-  PasscodeSettings 

Object

# PasscodeSettings

The declaration to configure passcode policy settings.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object PasscodeSettings
```

## Properties

`ChangeAtNextAuth`

`boolean`

If `true`, the system forces a password reset the next time the user tries to authenticate. If you set this key in a configuration in the system scope (device channel), the setting takes effect for all users, and admin authentication may fail until the admin user password is also reset.

Default: `false`

`CustomRegex`

PasscodeSettingsCustomRegexObject

Specifies a regular expression, and its description, to enforce password compliance. Use the simpler passcode settings whenever possible, and rely on regular expression matching only when necessary. Mistakes in regular expressions can lead to frustrating user experiences, such as unsatisfiable passcode policies, or policy descriptions that don’t match the enforced policy.

`FailedAttemptsResetInMinutes`

`integer`

The number of minutes before the login is reset after the maximum number of failed attempts. Also set the `MaximumFailedAttempts` key for this to take effect.

`MaximumFailedAttempts`

`integer`

The number of failed passcode attempts that the system allows the user before iOS erases the device or macOS locks the device. If you don’t change this setting, after six failed attempts, the device imposes a time delay before the user can enter a passcode again. The time delay increases with each failed attempt.

After the final failed attempt, the system securely erases all data and settings from the iOS device. A macOS device locks after the final attempt. The passcode time delay begins after the sixth attempt, so if this value is six or lower, the system has no time delay and triggers the erase or lock as soon as the user exceeds the limit.

Default: `11`

Minimum: `2`

Maximum: `11`

`MaximumGracePeriodInMinutes`

`integer`

The maximum period that a user can select, during which the user can unlock the device without a passcode. A value of `0` means no grace period, and the device requires a passcode immediately. In the absence of this key, the user can select any period. In macOS, the system translates this to screensaver settings.

`MaximumInactivityInMinutes`

`integer`

The maximum period that a user can select, during which the device can be idle before the system automatically locks it. When the device reaches this limit, the device locks and the user must enter the passcode to unlock it. In the absence of this key, the user can select any period. In macOS, the system translates this to screensaver settings.

Minimum: `0`

Maximum: `15`

`MaximumPasscodeAgeInDays`

`integer`

Specifies the maximum number of days that the passcode can remain unchanged. After this number of days, the system forces the user to change the passcode before it unlocks the device.

Minimum: `0`

Maximum: `730`

`MinimumComplexCharacters`

`integer`

Specifies the minimum number of complex characters in the password. A complex character is a character other than a number or a letter, such as `&`, `%`, `$`, and `#`.

Default: `0`

Minimum: `0`

Maximum: `4`

`MinimumLength`

`integer`

The minimum number of characters a passcode can contain.

Default: `0`

Minimum: `0`

Maximum: `16`

`PasscodeReuseLimit`

`integer`

The number of historical passcode entries the system checks when vaildating a new passcode. The device refuses a new passcode if it matches a previously used passcode within the specified passcode history range. In the absence of this key, the system performs no historical check.

Minimum: `1`

Maximum: `50`

`RequireAlphanumericPasscode`

`boolean`

If `true`, the passcode needs to consist of at least one alphabetic character and at least one number.

Default: `false`

`RequireComplexPasscode`

`boolean`

If `true`, the system requires a complex passcode. A complex passcode is one that doesn’t contain repeated characters or increasing or decreasing characters (such as 123 or CBA), and must contain at least one nonnumeric and nonalphabetic character.

Default: `false`

`RequirePasscode`

`boolean`

If `true`, the system requires the user to set a passcode without any requirements about the length or quality of the passcode. The presence of any other keys implicitly requires a passcode, and overrides this key’s value.

Default: `false`

## Discussion

Specify `com.apple.configuration.passcode.settings` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS, watchOS |
|------------------------------|---------------------|
| Allowed in User Enrollment   | iOS                 |
| Allowed in Local Enrollment  | iOS, macOS, watchOS |
| Allowed in System Scope      | iOS, macOS, watchOS |
| Allowed in User Scope        | macOS               |

## Topics

### Supporting Objects

object PasscodeSettingsCustomRegexObject

A regular expression and its description to enforce password compliance.

object PasscodeSettingsCustomRegex_DescriptionObject

A dictionary that contains supported OS language IDs for the keys and values that represent a localized description of the policy that the regular expression enforces.

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

object AccountExchange

The declaration to configure an Exchange account.

object AccountGoogle

The declaration to configure a Google account.

object AccountLDAP

The declaration to configure a Lightweight Directory Access Protocol (LDAP) account.

object AccountMail

The declaration to configure a Mail account.

object AccountSubscribedCalendar

The declaration to configure a Calendar subscription.

object AppManaged

The declaration to configure a managed app.

object DiskManagementSettings

The declaration to configure disk management settings on the device.

object LegacyInteractiveProfile

The declaration to configure an interactive, legacy profile.

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object SafariExtensionSettings

The declaration to configure Safari Extensions.

