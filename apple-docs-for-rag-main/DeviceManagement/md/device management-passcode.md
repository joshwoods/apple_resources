

- Device Management
-  Passcode 

Device Management Profile

# Passcode

The payload you use to configure a passcode policy.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object Passcode
```

## Properties

`allowSimple`

`boolean`

If `false`, the system prevents use of a simple passcode. A simple passcode contains repeated characters, or increasing or decreasing characters, such as `123` or `CBA`.

Default: `true`

`changeAtNextAuth`

`boolean`

If `true`, the system causes a password reset to occur the next time the user tries to authenticate. If this key is set in a device profile, the setting takes effect for all users, and admin authentications may fail until the admin user password is also reset. Available in macOS 10.13 and later.

Default: `false`

`customRegex`

Passcode.CustomRegex

Specifies a regular expression, and its description, used to enforce password compliance. Use the simpler passcode restrictions whenever possible, and rely on regular expression matching only when necessary. Mistakes in regular expressions can lead to frustrating user experiences, such as unsatisfiable passcode policies, or policy descriptions that don’t match the enforced policy.

Available in macOS 14 and later.

`forcePIN`

`boolean`

If `true`, the system forces the user to enter a PIN.

Default: `false`

`maxFailedAttempts`

`integer`

The number of allowed failed attempts to enter the passcode at the device’s lock screen. After four failed attempts, the system imposes a time delay before a passcode can be entered again. The delay increases with each attempt. In macOS, set `minutesUntilFailedLoginReset` to define a delay before the next passcode can be entered. When this number is exceeded in macOS, the system locks the device; in iOS, the system wipes the device.

Default: `11`

Minimum: `2`

Maximum: `11`

`maxGracePeriod`

`integer`

The maximum grace period, in minutes, to unlock the phone without entering a passcode. The default is `0`, which is no grace period and requires a passcode immediately. In macOS, the system translates this grace period value to screen-saver settings.

Default: `0`

`maxInactivity`

`integer`

The maximum number of minutes for which the device can be idle without the user unlocking it, before the system locks it. When this limit is reached, the system locks the device and the passcode is required to unlock it. The user can edit this setting, but the value can’t exceed the `maxInactivity` value.

In macOS, the system translates this inactivity value to screen-saver settings. The maximum value for macOS is `60`.

Setting this key removes the `never` option in the Settings UI on user enrolled devices.

Minimum: `0`

Maximum: `15`

`maxPINAgeInDays`

`integer`

The number of days for which the passcode can remain unchanged. After this number of days, the system forces the user to change the passcode before it unlocks the device.

Minimum: `0`

Maximum: `730`

`minComplexChars`

`integer`

The minimum number of complex characters that a passcode needs to contain. A *complex* character is a character other than a number or a letter, such as `&`, `%`, `$`, and `#`.

The system ignores this property for User Enrollments.

Default: `0`

Minimum: `0`

Maximum: `4`

`minLength`

`integer`

The minimum overall length of the passcode. This value is independent of the value for `minComplexChars`.

Default: `0`

Minimum: `0`

Maximum: `16`

`minutesUntilFailedLoginReset`

`integer`

The number of minutes before the system resets the login after the maximum number of unsuccessful login attempts is reached. This key requires setting `maxFailedAttempts`. Available in macOS 10.10 and later.

`pinHistory`

`integer`

This value defines *N*, where the new passcode must be unique within the last *N* entries in the passcode history.

Minimum: `1`

Maximum: `50`

`requireAlphanumeric`

`boolean`

If `true`, the system requires alphabetic characters instead of only numeric characters.

Default: `false`

## Discussion

Specify `com.apple.mobiledevice.passwordpolicy` as the payload type.

The presence of this payload type prompts an iOS or macOS device to present the user with a passcode entry mechanism. The complexity of the passcode can be customized with this payload.

On iOS User Enrollments, the system allows the Passcode payload type, but ignores all keys. Instead, the presence of the Passcode payload forces these settings:

- `allowSimple` = `false`

- `forcePIN` = `true`

- `minLength` = `6`

### Profile Availability

|                            |                     |
|----------------------------|---------------------|
| Device Channel             | iOS, macOS, watchOS |
| User Channel               | \-                  |
| Allow Manual Install       | iOS, macOS, watchOS |
| Requires Supervision       | \-                  |
| Requires User Approved MDM | \-                  |
| Allowed in User Enrollment | iOS                 |
| Allow Multiple Payloads    | iOS, macOS, watchOS |

### Profile Example

```

    PayloadContent

            allowSimple

            forcePIN

            maxFailedAttempts
            5
            maxGracePeriod
            1
            maxInactivity
            2
            maxPINAgeInDays
            30
            minLength
            8
            pinHistory
            2
            requireAlphanumeric

            PayloadIdentifier
            com.example.mypasscodepayload
            PayloadType
            com.apple.mobiledevice.passwordpolicy
            PayloadUUID
            2a8a75e5-d17d-44d5-b062-3cb92161af9f
            PayloadVersion
            1

    PayloadDisplayName
    Passcode
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    e044f50d-ff67-4bcd-9f3f-d7b678091061
    PayloadVersion
    1

```

## Topics

### Profiles

object Passcode.CustomRegex

The regex defining the passcode policy.

## See Also

### Security

object SecurityPreferences

The payload you use to configure security preferences.

object SmartCard

The payload you use to configure a smart card.

