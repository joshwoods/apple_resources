

- Device Management
-  SystemPolicyManaged 

Device Management Profile

# SystemPolicyManaged

The payload you use to configure the Finder’s contextual menu to bypass the system policy.

macOS 10.8+Device Assignment ServicesVPP License Management

``` source
object SystemPolicyManaged
```

## Properties

`DisableOverride`

`boolean`

If `true`, disables the Finder’s contextual menu item.

Default: `false`

## Discussion

Specify `com.apple.systempolicy.managed` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            DisableOverride

            PayloadIdentifier
            com.example.mysystempolicymanagedpayload
            PayloadType
            com.apple.systempolicy.managed
            PayloadUUID
            4ceaeaba-dfb9-4eb2-a641-a89c472856f0
            PayloadVersion
            1

    PayloadDisplayName
    System Policy Managed
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4899fa10-e6e6-4d74-9fa3-64a2feb57c8e
    PayloadVersion
    1

```

## See Also

### System Policy

object SystemPolicyControl

The payload you use to configure the system policy for assessments.

object SystemPolicyKernelExtensions

The payload you use to configure the kernel extension policies.

object SystemPolicyRule

The payload you use to configure the system policy.

