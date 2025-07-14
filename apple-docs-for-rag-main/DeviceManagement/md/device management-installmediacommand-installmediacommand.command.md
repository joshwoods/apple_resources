

- Device Management
- InstallMediaCommand
-  InstallMediaCommand.Command 

Device Management Command

# InstallMediaCommand.Command

The request dictionary to install a book.

iOS 8.0+iPadOS 8.0+macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object InstallMediaCommand.Command
```

## Properties

`Author`

`string`

The name of the book’s author. This value is available in iOS 8 and later.

`iTunesStoreID`

`integer`

The book’s iTunes Store identifier.

`Kind`

`string`

The kind of the media, which can be one of the following values:

- `pdf`: A PDF file

- `epub`: An EPUB file in `gzip` format.

- `ibooks`: An iBooks Author file in `gzip` format.

If you omit this value, its value is the file extension in the URL. This value is available in iOS 8 and later.

Possible Values: `pdf, epub, ibooks`

`MediaURL`

`string`

The URL to retrieve the book. This value is available in iOS 8 and later.

`MediaType`

`string`

 (Required) 

The media type, which can only be `Book`.

Value: `Book`

`PersistentID`

`string`

The book’s persistent identifier in reverse-DNS form; for example, `com.acme.manuals.training`. This value is available in iOS 8 and later.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to install a book.

Value: `InstallMedia`

`Title`

`string`

The book’s title. This value is available in iOS 8 and later.

`Version`

`string`

The book’s version number. This value is available in iOS 8 and later.

