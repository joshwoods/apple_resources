

- Device Management
-  List Active NSExtensions 

Web Service Endpoint

# List Active NSExtensions

Get a list of active extensions for a user on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ActiveNSExtensionsCommand
```

## HTTP Body

ActiveNSExtensionsCommand

The command to get a list of active extensions for a user on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ActiveNSExtensionsResponse

`OK`

A response from the device after it processes the command to get a list of active extensions for a user.

Content-Type: application/xml

## Discussion

This command returns information about the active extensions for a user. Extensions exist for each user, not for the device.

Extensions restricted from executing by Application Launch Restrictions or the NSExtensionManagement configuration profile won’t appear in the response.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

|                            |                    |
|----------------------------|--------------------|
| Device Channel             | \-                 |
| User Channel               | macOS              |
| Requires Supervision       | \-                 |
| Allowed in User Enrollment | \-                 |
| Required Access Right      | QueryInstalledApps |

### Example Request and Response

- Request
- Response

```

    Command

        FilterExtensionPoints

            com.apple.share-services

        RequestType
        ActiveNSExtensions

    CommandUUID
    0001_ActiveNSExtensions

```

```

    ActiveNSExtensions

            ContainerDisplayName
            Messages.app
            ContainerIdentifier
            com.apple.iChat
            DisplayName
            Messages
            ExtensionPoint
            com.apple.share-services
            Identifier
            com.apple.messages.ShareExtension
            Path
            /System/Applications/Messages.app/Contents/PlugIns/Messages Share Extension.appex
            UserElection
            Use
            Version
            1.0

            DisplayName
            Set Background Image
            ExtensionPoint
            com.apple.share-services
            Identifier
            com.apple.share.System.set-desktop-image
            Path
            /System/Library/PrivateFrameworks/ShareKit.framework/Versions/A/PlugIns/SystemSetDesktopImage.appex
            UserElection
            Use
            Version
            639

            DisplayName
            Add to Reading List
            ExtensionPoint
            com.apple.share-services
            Identifier
            com.apple.share.System.add-to-safari-reading-list
            Path
            /System/Library/PrivateFrameworks/ShareKit.framework/Versions/A/PlugIns/SystemAddToReadingList.appex
            UserElection
            Use
            Version
            639

    CommandUUID
    0001_ActiveNSExtensions
    NotOnConsole

    Status
    Acknowledged
    UDID
    E84CD517-CB37-52F7-988C-DB5137B604B8
    UserID
    03EBB586-53E7-48CE-8E6E-C54A374F6FA6
    UserLongName
    admin
    UserShortName
    admin

```

## Topics

### Command and Response

object ActiveNSExtensionsCommand

The command to get a list of active extensions for a user on a device.

object ActiveNSExtensionsResponse

A response from the device after it processes the command to get a list of active extensions for a user.

## See Also

### Extensions

List the NSExtensions

Get a list of the installed extensions for a user on a device.

