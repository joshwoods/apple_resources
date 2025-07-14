

- Device Management
-  SystemPolicyRule 

Device Management Profile

# SystemPolicyRule

The payload you use to configure the system policy.

macOS 10.8+Device Assignment ServicesVPP License Management

``` source
object SystemPolicyRule
```

## Properties

`Comment`

`string`

This string appears in the System Policy UI. If it’s missing, `PayloadDisplayName` or `PayloadDescription` is entered into this field before the rule is added to the System Policy database.

`Expiration`

`date`

The expiration date for rules being processed.

`LeafCertificate`

`data`

The single leaf certificate for the app that is in the allow list.

`OperationType`

`string`

The type of operation.

Default: `operation:execute`

Possible Values: `operation:execute, operation:install, operation:lsopen`

`Priority`

`number`

The rule’s priority.

`Requirement`

`string`

The policy requirement. This key must follow the syntax described in Code Signing Requirement Language.

## Discussion

Specify `com.apple.systempolicy.rule` as the payload type.

This payload allows control over Gatekeeper’s system policy rules. The keys and functionality are tightly related to the `spctl` command line tool. For more information, see the manual page for `spctl`.

This payload must only exist in a device profile. If the payload is present in a user profile, an error is generated during installation and the profile installation fails.

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

            Priority
            101
            Requirement
            anchor apple generic and identifier "com.example.myapp" and (certificate leaf[field.9.8.765.432109.876.5.4.3] /* exists */ or certificate 1[field.1.2.840.113635.100.6.2.6] /* exists */ and certificate leaf[field.9.8.765.432109.876.5.4.3] /* exists */ and certificate leaf[subject.OU] = "ABCDE12345")
            PayloadIdentifier
            com.example.mysystempolicyrulepayload
            PayloadType
            com.apple.systempolicy.rule
            PayloadUUID
            624b5152-a1cd-4bac-baa3-51fbb1f04973
            PayloadVersion
            1

    PayloadDisplayName
    System Policy Rule
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    7fa54f02-e6e1-4042-bb75-a2a4d962ac6d
    PayloadVersion
    1

```

## See Also

### System Policy

object SystemPolicyControl

The payload you use to configure the system policy for assessments.

object SystemPolicyKernelExtensions

The payload you use to configure the kernel extension policies.

object SystemPolicyManaged

The payload you use to configure the Finder’s contextual menu to bypass the system policy.

