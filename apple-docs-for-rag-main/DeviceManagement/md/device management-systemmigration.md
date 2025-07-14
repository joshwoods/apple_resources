

- Device Management
-  SystemMigration 

Device Management Profile

# SystemMigration

The payload you use to configure system migration.

macOS 10.12.4+Device Assignment ServicesVPP License Management

``` source
object SystemMigration
```

## Properties

`CustomBehavior`

`[`SystemMigration.CustomBehaviorItem`]`

The list of custom behavior dictionaries.

## Discussion

Specify `com.apple.systemmigration` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            CustomBehavior

                    Context
                    Windows
                    Paths

                            SourcePath
                            C:/Users/Documents
                            TargetPath
                            ~/Users/Documents
                            SourcePathInUserHome

                            TargetPathInUserHome

            PayloadIdentifier
            com.example.mysystemmigrationpayload
            PayloadType
            com.apple.systemmigration
            PayloadUUID
            553d6db9-2704-4127-8384-003926e5b813
            PayloadVersion
            1

    PayloadDisplayName
    System Migration
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    75157e67-d7ff-44ec-9ccf-8496be33864a
    PayloadVersion
    1

```

## Topics

### Objects

object SystemMigration.CustomBehaviorItem

The custom behavior dictionary.

object SystemMigration.CustomBehaviorItem.PathsItem

The custom behavior path dictionary.

## See Also

### System Updates

object SoftwareUpdate

The payload you use to configure the software update policy.

