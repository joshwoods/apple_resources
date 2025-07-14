

- Device Management
-  Profile 

Object

# Profile

A profile’s properties and their values.

Device Assignment ServicesVPP License Management

``` source
object Profile
```

## Properties

`allow_pairing`

`boolean`

Default is `true`. In iOS 13, this property was deprecated.

`anchor_certs`

`[string]`

An array of strings, where each string is a DER-encoded (Distinguished Encoding Rules) certificate converted to Base64 encoding. If provided, the device uses these certificates as trusted anchor certificates when evaluating the trust of the connection to the MDM server URL. Otherwise, the device uses the built-in root certificates.

`auto_advance_setup`

`boolean`

If set to `true`, the device will tell Setup Assistant to automatically advance though its screens. Default is `false`.

This key is valid in X-Server-Protocol-Version 2 and later.

Available on tvOS and macOS 11 and later.

`await_device_configured`

`boolean`

If `true`, the device will not continue in Setup Assistant until the MDM server sends a command that states the device is configured (see Release Device from Await Configuration). Default is `false`. Ignored on iOS devices if `is_supervised` is `false`. This key is valid in X-Server-Protocol-Version 2 and later.

`configuration_web_url`

`string`

The URL that the clients load into a web view during setup. This site provides the appropriate UI to authenticate the user, and when satisfied, initiates the download of the MDM enrollment profile.

To provide the MDM enrollment profile, the web view looks for a page with MIME type `application/x-apple-aspen-config`.

While the user is allowed to navigate to any site or host during authentication, the MDM enrollment profile must originate from the same host as specified in this field.

`department`

`string`

The user-defined department or location name.

`devices`

`[string]`

Array of strings that contains device serial numbers (may be empty).

`is_mandatory`

`boolean`

If `true`, the user may not skip applying the profile returned by the MDM server. Default is `false`.

In iOS 13 and later, all DEP enrollments are mandatory.

`is_mdm_removable`

`boolean`

If `false`, the MDM payload delivered by the configuration URL cannot be removed by the user via the user interface on the device; that is, the MDM payload is locked onto the device. This key can be set to `false` only if `is_supervised` is set to `true`. Defaults to `true`.

`is_multi_user`

`boolean`

If `true`, tells the device to configure for Shared iPad. Default is false. This key is valid only for Apple School Manager or Apple Business Manager organizations using X-Server-Protocol-Version 2 and later.

Devices that do not meet the Shared iPad minimum requirements do not honor this command. With iOS devices, `com.apple.mdm.per-user-connections` must be added to the MDM enrollment profile’s Server Capabilities.

`is_supervised`

`boolean`

If `true`, the device must be supervised. Defaults to `false`.

In iOS 11, DEP devices that are not supervised have been deprecated.

In iOS 13, all DEP devices will be supervised and the OS will ignore the `is_supervised` flag completely.

`language`

`string`

A language designator is a code that represents a language.

Use the two-letter ISO 639-1 standard (preferred) or the three-letter ISO 639-2 standard. If an ISO 639-1 code is not available for a particular language, use the ISO 639-2 code instead.

See Language and Locale IDs for more information.

Example two-letter: `en`, `fr`, `ja`

Example three-letter: `eng`, `fre`, `jpn`, `haw`

Available on tvOS and macOS 11 and later.\`\`

`org_magic`

`string`

A string that uniquely identifies various services that are managed by a single organization.

`profile_name`

`string`

A human-readable name for the profile.

`region`

`string`

A region designator is a code that represents a country. Available on tvOS and macOS 11 and later.

Use the ISO 3166-1 standard, a two-letter, capitalized code.

Examples: US, GB, AU

`skip_setup_items`

`[string]`

A list of setup panes to skip. The list of valid strings is defined in SkipKeys.

`supervising_host_certs`

`[string]`

Each string contains a DER-encoded certificate converted to Base64 encoding. If provided, the device will continue to pair with a host that possesses one of these certificates even when `allow_pairing` is set to `false`. If `is_supervised` is `false`, this list is unused.

`support_email_address`

`string`

A support email address for the organization. This key is valid in X-Server-Protocol-Version 2 and later.

`support_phone_number`

`string`

A support phone number for the organization.

`url`

`string`

String. The URL of the MDM server.

## Mentioned in 

Authenticating Through Web Views

## Topics

### Skip Keys

object SkipKeys

The list of setup panes.

## See Also

### Objects and Data Types

object Device

A device’s properties and their values.

object MachineInfo

A device’s information in response to a MDM enrollment profile request.

object Limit

A ranged limit.

object Url

A URL object.

