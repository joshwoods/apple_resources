

- Device Management
-  SystemPolicyKernelExtensions 

Device Management Profile

# SystemPolicyKernelExtensions

The payload you use to configure the kernel extension policies.

macOS 10.13.2+Device Assignment ServicesVPP License Management

``` source
object SystemPolicyKernelExtensions
```

## Properties

`AllowedKernelExtensions`

SystemPolicyKernelExtensions.AllowedKernelExtensions

The dictionary that represents a set of kernel extensions that the system always allows to load on the computer. The dictionary maps team identifiers (keys) to arrays of bundle identifiers.

`AllowNonAdminUserApprovals`

`boolean`

If `true`, nonadministrative users can approve additional kernel extensions in the Security & Privacy preferences.

Available in macOS 11 and later.

Default: `false`

`AllowedTeamIdentifiers`

`[string]`

The array of team identifiers that define which validly signed kernel extensions can load.

`AllowUserOverrides`

`boolean`

If `true`, users can approve additional kernel extensions that configuration profiles don’t explicitly allow.

Default: `false`

## Discussion

Specify `com.apple.syspolicy.kernel-extension-policy` as the payload type.

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

            AllowUserOverrides

            AllowedTeamIdentifiers

                ABCDE12345

            AllowedKernelExtensions

                    com.example.mydriver

                ABCDE12345

                    com.example.kext.mydriver

            PayloadIdentifier
            com.example.mysystempolicykernalextensionspayload
            PayloadType
            com.apple.syspolicy.kernel-extension-policy
            PayloadUUID
            3202f59b-3583-4e6c-82ae-776f3c815df1
            PayloadVersion
            1

    PayloadDisplayName
    System Policy Kernal Extension
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    d9fa7f5b-713d-48f8-a8bd-219cf3061873
    PayloadVersion
    1

```

## Topics

### Objects

object SystemPolicyKernelExtensions.AllowedKernelExtensions

The dictionary that represents a set of kernel extensions.

## See Also

### System Policy

object SystemPolicyControl

The payload you use to configure the system policy for assessments.

object SystemPolicyManaged

The payload you use to configure the Finder’s contextual menu to bypass the system policy.

object SystemPolicyRule

The payload you use to configure the system policy.

