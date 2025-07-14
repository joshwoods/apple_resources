

- Device Management
-  List the NSExtensions 

Web Service Endpoint

# List the NSExtensions

Get a list of the installed extensions for a user on a device.

macOS 10.13+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#NSExtensionMappingsCommand
```

## HTTP Body

NSExtensionMappingsCommand

The command to get a list of the installed extensions for a user on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

NSExtensionMappingsResponse

`OK`

A response from the device after it processes the command to get a list of the installed extensions for a user.

Content-Type: application/xml

## Discussion

This list is a superset of the list that ActiveNSExtensionsCommand returns. It may contain extensions that the system never enables due to various restrictions.

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

        RequestType
        NSExtensionMappings

    CommandUUID
    0001_NSExtensionMappings

```

```

    CommandUUID
    0001_NSExtensionMappings
    NSExtensionMappings

            DisplayName
            Photos
            ExtensionPoint
            com.apple.storagemanagement
            Identifier
            com.apple.Photos.StorageManagementExtension

            DisplayName
            Messages
            ExtensionPoint
            com.apple.share-services
            Identifier
            com.apple.messages.ShareExtension

            DisplayName
            iCloud Drive
            ExtensionPoint
            com.apple.fileprovider-nonui
            Identifier
            com.apple.CloudDocs.MobileDocumentsFileProvider

            DisplayName
            Notes Spotlight Index Extension
            ExtensionPoint
            com.apple.spotlight.index
            Identifier
            com.apple.Notes.SpotlightIndexExtension

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

object NSExtensionMappingsCommand

The command to get a list of the installed extensions for a user on a device.

object NSExtensionMappingsResponse

A response from the device after it processes the command to get a list of the installed extensions for a user.

## See Also

### Extensions

List Active NSExtensions

Get a list of active extensions for a user on a device.

