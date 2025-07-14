

- Device Management
-  SystemPolicyControl 

Device Management Profile

# SystemPolicyControl

The payload you use to configure the system policy for assessments.

macOS 10.8+Device Assignment ServicesVPP License Management

``` source
object SystemPolicyControl
```

## Properties

`AllowIdentifiedDevelopers`

`boolean`

If `true`, enables Gatekeeper’s “Mac App Store and identified developers” option.

If `false`, enables Gatekeeper’s “Mac App Store” option.

If the value of `EnableAssessment` isn’t set to `true`, this key has no effect.

`EnableAssessment`

`boolean`

If `true`, enables Gatekeeper. If `false`, disables Gatekeeper.

`EnableXProtectMalwareUpload`

`boolean`

If `false`, prevents Gatekeeper from prompting the user to upload blocked malware to Apple for purposes of improving malware detection.

## Discussion

Specify `com.apple.systempolicy.control` as the payload type.

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

            AllowIdentifiedDevelopers

            EnableAssessment

            PayloadIdentifier
            com.example.mysystempolicycontrolpayload
            PayloadType
            com.apple.systempolicy.control
            PayloadUUID
            f26fc0a5-09f4-4d71-9a5c-6f1a7d30e905
            PayloadVersion
            1

    PayloadDisplayName
    System Policy Control
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    f379ac8d-8b9e-4e36-98e7-a43094d51e38
    PayloadVersion
    1

```

## See Also

### System Policy

object SystemPolicyKernelExtensions

The payload you use to configure the kernel extension policies.

object SystemPolicyManaged

The payload you use to configure the Finder’s contextual menu to bypass the system policy.

object SystemPolicyRule

The payload you use to configure the system policy.

