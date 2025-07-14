

- Device Management
-  SystemExtensions 

Device Management Profile

# SystemExtensions

The payload you use to configure system extensions.

macOS 10.15+Device Assignment ServicesVPP License Management

``` source
object SystemExtensions
```

## Properties

`AllowedSystemExtensions`

SystemExtensions.AllowedSystemExtensions

A dictionary of approved system extensions on the computer. The dictionary maps the team identifiers (keys) to arrays of bundle identifiers, where the bundle identifier defines the system extension to install.

To avoid requiring an administrator to authorize the operation, you can activate system extensions that this key specifies using activationRequest(forExtensionWithIdentifier:queue:).

It’s an error for the same team identifier to appear in both the `AllowedTeamIdentifiers` array and as a key in this dictionary.

`AllowedSystemExtensionTypes`

SystemExtensions.AllowedSystemExtensionTypes

A dictionary that maps a team identifier to an array of strings, where each string is a type of system extension that you can install for that team identifier. The allowed extension types are `DriverExtension`, `NetworkExtension`, and `EndpointSecurityExtension`.

If there’s no entry for a specified team identifier in the dictionary, the system allows all extension types.

`AllowedTeamIdentifiers`

`[string]`

An array of team identifiers that defines valid, signed system extensions that are allowable to load. Approved system extensions are those signed with any of the specified team identifiers.

To avoid requiring an administrator to authorize the operation, you can activate system extensions that this key specifies using activationRequest(forExtensionWithIdentifier:queue:).

It’s an error for the same team identifier to appear in both this array and as a key in the `AllowedSystemExtensions` dictionary.

`AllowUserOverrides`

`boolean`

If `false`, restricts users from approving additional system extensions that configuration profiles don’t explicitly allow.

Default: `true`

`NonRemovableFromUISystemExtensions`

SystemExtensions.NonRemovableFromUISystemExtensions

A dictionary of system extensions on the computer. The dictionary maps the team identifiers (keys) to arrays of bundle identifiers, where the bundle identifier defines the system extension which can’t be disabled or uninstalled from System Settings or Finder. The set of system extensions between `RemovableSystemExtensions` and `NonRemovableFromUISystemExtensions` can to overlap.

`NonRemovableSystemExtensions`

SystemExtensions.NonRemovableSystemExtensions

A dictionary of system extensions on the computer. The dictionary maps the team identifiers (keys) to arrays of bundle identifiers, where the bundle identifier defines the system extension which can’t be disabled or uninstalled when SIP is enabled. It’s an error for the same mapping to appear in the dictionary values corresponding to ‘`RemovableSystemExtensions`’ and ‘`NonRemovableSystemExtensions`’ keys.

`RemovableSystemExtensions`

SystemExtensions.RemovableSystemExtensions

A dictionary of system extensions that are allowed to remove themselves from the machine. The dictionary maps team identifiers (keys) to arrays of bundle identifiers, where the bundle identifier defines the system extension. An application using the `OSSystemExtensionDeactivationRequest` API can deactivate the specified system extensions without requiring an administrator to authorize the operation.

Available in macOS 12 and later.

## Discussion

Specify `com.apple.system-extension-policy` as the payload type.

When there are multiple installed profiles, the keys combine as follows:

- `AllowUserOverrides` is `false` if any profile sets it to `false`.

- All the other values combine together.

Beginning in macOS 11.3, installing or removing this payload can change the state of system extensions on the computer. If a containing application activates a system extension, and the system extension is in a pending state, installing a payload that allows the extension completes the activation process. If a system extension is active, removing a payload that allows the extension deactivates that extension.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | \-    |
| Requires Supervision       | \-    |
| Requires User Approved MDM | macOS |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            AllowedExtensions

                com.apple.share.System.send

            PayloadIdentifier
            com.example.mysystemextensionpayload
            PayloadType
            com.apple.nsextension
            PayloadUUID
            3b378001-8cff-4bde-a6af-843fdb02f36d
            PayloadVersion
            1

    PayloadDisplayName
    System Extensions
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2e880ad8-e49e-47af-b416-7e6c3fba9df2
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object SystemExtensions.AllowedSystemExtensionTypes

A dictionary that maps team identifiers to system extensions.

object SystemExtensions.AllowedSystemExtensions

A dictionary that maps team identifiers to bundle identifiers that are allowed.

object SystemExtensions.NonRemovableFromUISystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.NonRemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are non-removable.

object SystemExtensions.RemovableSystemExtensions

A dictionary that maps team identifiers to bundle identifiers of extensions that are removable.

## See Also

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object EnergySaver

The payload you use to configure energy-saver settings.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

