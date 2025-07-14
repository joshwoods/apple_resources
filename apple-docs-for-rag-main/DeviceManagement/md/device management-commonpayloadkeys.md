

- Device Management
-  CommonPayloadKeys 

Device Management Profile

# CommonPayloadKeys

The payload properties that are common across all profiles.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+Device Assignment ServicesVPP License Management

``` source
object CommonPayloadKeys
```

## Properties

`PayloadDescription`

`string`

The human-readable description of this payload. This description appears on the Detail screen.

`PayloadDisplayName`

`string`

The human-readable name for the profile payload. The name appears on the Detail screen and doesn’t need to be unique.

`PayloadIdentifier`

`string`

 (Required) 

The reverse-DNS-style identifier for the payload. This identifier is usually the same as the TopLevel value, with an additional appended component. This string must be unique within the profile.

During a profile replacement, the system updates payloads with the same `PayloadIdentifier` and `PayloadUUID` in the old and new profiles.

`PayloadOrganization`

`string`

The human-readable string containing the name of the organization that provides the profile. This value doesn’t need to match the organization payload value in the enclosing dictionary.

`PayloadType`

`string`

 (Required) 

The payload type, which each payload domain’s reference page specifies.

`PayloadUUID`

`string`

 (Required) 

The globally unique identifier for the payload. The actual content is unimportant, but must be globally unique. In macOS, use `uuidgen` to generate UUIDs.

During a profile replacement, the system updates payloads with the same `PayloadIdentifier` and `PayloadUUID` in the old and new profiles.

`PayloadVersion`

`integer`

 (Required) 

The version of this specific payload.

Value: `1`

## Discussion

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | \-                                     |

## See Also

### Top Level

object TopLevel

The top-level payload properties you use to configure all profiles.

