

- Device Management
-  Install Media 

Web Service Endpoint

# Install Media

Install a book on a device.

iOS 8.0+iPadOS 8.0+macOS 10.9+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstallMediaCommand
```

## HTTP Body

InstallMediaCommand

The command to install a book on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstallMediaResponse

`OK`

A response from the device after it processes the command to install a book.

Content-Type: application/xml

## Discussion

The request must contain either the `iTunesStoreID` or `MediaURL`. The `MediaURL` must lead to a PDF file, an EPUB file in `gzip` format, or an iBooks Author document in `gzip` format. Books that MDM has installed become managed books.

Use Volume Purchase Program (VPP) Licensing to obtain books from the Book Store. Books from the Book Store require that the device has enabled App Store. These books undergo backup, sync with iTunes, and remain on the device after removal of the MDM profile.

Books that aren’t from the Book Store don’t require that the device has enabled App Store. These books don’t undergo backup, don’t sync with iTunes, and don’t remain on the device after removal of the MDM profile.

If the book already exists, this command updates the book and makes it visable to the MDM server. The user doesn’t receive a prompt for a book installation or update unless they need to log in to complete a Book Store transaction.

If you install a book from the Book Store with the same `iTunesStoreID` as an existing managed book, the new book replaces the existing one.

If you install a book that isn’t from the Book Store with the same `PersistentID` as an existing book that also isn’t from the Book Store, the new book replaces the existing one.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                      |
|----------------------------|----------------------|
| Device Channel             | iOS, Shared iPad     |
| User Channel               | macOS                |
| Requires Supervision       | \-                   |
| Allowed in User Enrollment | iOS                  |
| Required Access Right      | AllowAppInstallation |

### Example Request and Response (Enterprise Book)

- Request
- Response

```

    Command

        Author
        Acme, Inc.
        Kind
        pdf
        MediaType
        Book
        MediaURL
        https://yourmdmhost.example.com/files/myenterprisebook.pdf
        PersistentID
        com.acme.pdf.myenterprisebook
        RequestType
        InstallMedia
        Title
        My Enterprise Book
        Version
        1.0

    CommandUUID
    0001_InstallMedia

```

```

    CommandUUID
    0001_InstallMedia
    MediaType
    Book
    MediaURL
    https://yourmdmhost.example.com/files/myenterprisebook.pdf
    PersistentID
    com.acme.pdf.myenterprisebook
    State
    Installing
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

### Example Request and Response (VPP Book)

- Request
- Response

```

    Command

        MediaType
        Book
        RequestType
        InstallMedia
        iTunesStoreID
        1420662672

    CommandUUID
    0001_InstallMedia

```

```

    CommandUUID
    0001_InstallMedia
    MediaType
    Book
    State
    Installing
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E
    iTunesStoreID
    1420662672

```

## Topics

### Command and Response

object InstallMediaCommand

The command to install a book on a device.

object InstallMediaResponse

A response from the device after it processes the command to install a book.

## See Also

### Managed Media

List the Managed Media

Get a list of the managed books on a device.

Remove Media

Remove a previously installed book from a device.

