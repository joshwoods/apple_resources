

- Device Management
-  LoginItemsManagedItems 

Device Management Profile

# LoginItemsManagedItems

The payload you use to configure a device’s login items.

macOS 10.13+Device Assignment ServicesVPP License Management

``` source
object LoginItemsManagedItems
```

## Properties

`AutoLaunchedApplicationDictionary-managed`

`[`LoginItemsManagedItems.LoginItem`]`

 (Required) 

An array of login item dictionaries.

## Discussion

Specify `com.apple.loginitems.managed` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            AutoLaunchedApplicationDictionary-managed

                    Path
                    /System/Applications/Example.app
                    Hide

            PayloadIdentifier
            com.example.myloginitemsmanageditemspayload
            PayloadType
            com.apple.loginitems.managed
            PayloadUUID
            f19d4636-fa34-4a7c-8e8b-e92de516c893
            PayloadVersion
            1

    PayloadDisplayName
    Login Items Managed Items
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    98128de8-d76c-44fa-9509-5601c0d66281
    PayloadVersion
    1

```

## Topics

### Objects

object LoginItemsManagedItems.LoginItem

A dictionary with the details about a login item.

## See Also

### Login

object LoginWindowLoginItems

The payload you use to configure login behavior.

object LoginWindow

The payload you use to configure login window behavior.

object LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

object ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

