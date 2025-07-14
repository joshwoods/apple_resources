

- Device Management
-  List the Managed Media 

Web Service Endpoint

# List the Managed Media

Get a list of the managed books on a device.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#ManagedMediaListCommand
```

## HTTP Body

ManagedMediaListCommand

The command to get a list of the managed books on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

ManagedMediaListResponse

`OK`

A response from the device after it processes the command to get a list of managed books.

Content-Type: application/xml

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Query Availability

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

    Command

        RequestType
        ManagedMediaList

    CommandUUID
    0001_ManagedMediaList

```

```

    Books

            Author
            Acme, Inc.
            Kind
            pdf
            PersistentID
            com.acme.pdf.myenterprisebook
            State
            Managed
            Title
            My Enterprise Book
            Version
            1.0

    CommandUUID
    0001_ManagedMediaList
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object ManagedMediaListCommand

The command to get a list of the managed books on a device.

object ManagedMediaListResponse

A response from the device after it processes the command to get a list of managed books.

## See Also

### Managed Media

Install Media

Install a book on a device.

Remove Media

Remove a previously installed book from a device.

