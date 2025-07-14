

- Device Management
-  ServiceManagementManagedLoginItems 

Device Management Profile

# ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

macOS 13.0+Device Assignment ServicesVPP License Management

``` source
object ServiceManagementManagedLoginItems
```

## Properties

`Rules`

`[`ServiceManagementManagedLoginItems.Rule`]`

 (Required) 

An array of service management rules.

## Discussion

Specify `com.apple.servicemanagement` as the payload type.

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

            PayloadIdentifier
            com.example.myservicemanagementpayload
            PayloadUUID
            0d4e2ece-dfa7-4103-97ff-e91a9f842a1d
            PayloadType
            com.apple.servicemanagement
            Rules

                    RuleType
                    BundleIdentifier
                    RuleValue
                    com.example.myapp
                    Comment
                    My Example App

                    RuleType
                    BundleIdentifierPrefix
                    RuleValue
                    com.example
                    Comment
                    All apps from Example

                    RuleType
                    Label
                    RuleValue
                    com.example.internal.tool
                    Comment
                    Job to run an internal task here at Example

                    RuleType
                    LabelPrefix
                    RuleValue
                    com.example
                    Comment
                    All jobs to run internal tasks here at Example

                    RuleType
                    TeamIdentifier
                    RuleValue
                    ABCDE12345
                    Comment
                    Another way to specify all apps from Example

    PayloadDisplayName
    Service Management
    PayloadIdentifier
    com.example.myprofile
    PayloadUUID
    03cca12c-a610-44c2-96f9-fdabe3acd47d
    PayloadType
    Configuration
    PayloadScope
    System

```

## Topics

### Supporting Objects

object ServiceManagementManagedLoginItems.Rule

A dictionary that configures a service management rule.

## See Also

### Login

object LoginItemsManagedItems

The payload you use to configure a device’s login items.

object LoginWindowLoginItems

The payload you use to configure login behavior.

object LoginWindow

The payload you use to configure login window behavior.

object LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

