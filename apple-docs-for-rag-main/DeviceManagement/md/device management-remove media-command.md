

- Device Management
-  Remove Media 

Web Service Endpoint

# Remove Media

Remove a previously installed book from a device.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#RemoveMediaCommand
```

## HTTP Body

RemoveMediaCommand

The command to remove an installed book from a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

RemoveMediaResponse

`OK`

A response from the device after it processes the command to remove a book from a device.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                      |
|----------------------------|----------------------|
| Device Channel             | iOS, Shared iPad     |
| User Channel               | \-                   |
| Requires Supervision       | \-                   |
| Allowed in User Enrollment | iOS                  |
| Required Access Right      | AllowAppInstallation |

### Example Request and Response

- Request
- Response

```

    MediaType
    Book
    PersistentID
    com.acme.pdf.myenterprisebook
    RequestType
    RemoveMedia

```

```

    CommandUUID
    0001_RemoveMedia
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object RemoveMediaCommand

The command to remove an installed book from a device.

object RemoveMediaResponse

A response from the device after it processes the command to remove a book from a device.

## See Also

### Managed Media

Install Media

Install a book on a device.

List the Managed Media

Get a list of the managed books on a device.

