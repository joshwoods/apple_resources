

- Device Management
- RemoveMediaCommand
-  RemoveMediaCommand.Command 

Device Management Command

# RemoveMediaCommand.Command

The request dictionary to remove an installed book.

iOS 8.0+iPadOS 8.0+Device Assignment ServicesVPP License Management

``` source
object RemoveMediaCommand.Command
```

## Properties

`iTunesStoreID`

`string`

The book’s iTunes Store identifier.

`MediaType`

`string`

 (Required) 

The media type, which can only be `Book`.

Value: `Book`

`PersistentID`

`string`

The book’s persistent identifier in reverse-DNS form; for example, `com.acme.manuals.training`.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to remove an installed book.

Value: `RemoveMedia`

