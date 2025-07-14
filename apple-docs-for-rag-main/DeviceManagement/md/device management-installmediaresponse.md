

- Device Management
-  InstallMediaResponse 

Device Management Command

# InstallMediaResponse

A response from the device after it processes the command to install a book.

iOS 8.0+iPadOS 8.0+macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object InstallMediaResponse
```

## Properties

`CommandUUID`

`string`

The unique identifier of the command for this response.

`EnrollmentID`

`string`

 (Required) 

A per-enrollment device identifier for user enrollment.

`EnrollmentUserID`

`string`

 (Required) 

A per-enrollment user identifier for user enrollment.

`ErrorChain`

`[`InstallMediaResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`iTunesStoreID`

`integer`

The book’s iTunes Store identifier, if present in the command.

`MediaType`

`string`

The media type, which can only be `Book`.

`MediaURL`

`string`

The URL to retrieve the book, if present in the command. This value is available in iOS 8 and later.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`PersistentID`

`string`

The book’s persistent identifier, if present in the command. This value is available in iOS 8 and later.

`RejectionReason`

`string`

The reason, if installation fails, which is one of the following values:

- `CouldNotVerifyITunesStoreID`: The `iTunesStoreID` is invalid.

- `PurchaseNotFound`: The Volume Purchase Program (VPP) license isn’t in the user’s history.

- `AppStoreDisabled`: App Store isn’t available on the device.

- `WrongMediaType`: The media type is invalid. The only valid type is `Book`.

- `DownloadInvalid`: The URL doesn’t lead to a valid book.

- `EnterpriseBooksNotSupportedInMultiUser`: Multiuser mode doesn’t support enterprise books.

Possible Values: `CouldNotVerifyITunesStoreID, PurchaseNotFound, AppStoreDisabled, WrongMediaType, DownloadInvalid, EnterpriseBooksNotSupportedInMultiUser`

`Status`

`string`

 (Required) 

The status of the response, which is one of the following values:

- `Acknowledged`: The device processed the command successfully.

- `Error`: An error occurred. See the `ErrorChain` for more details.

- `CommandFormatError`: A protocol error occurred, which can result from a malformed command.

- `Idle`: The device is idle; there’s no status.

- `NotNow`: The device received the command, but couldn’t execute it.

Possible Values: `Acknowledged, Error, CommandFormatError, Idle, NotNow`

`State`

`string`

The installation state of this book. The `Failed` and `Unknown` states are transient and the device only reports them once. Books from the Book Store report their state as `Installed` instead of `Managed`.

Possible Values: `Queued, PromptingForLogin, Updating, Installing, Managed, ManagedButUninstalled, Installed, Uninstalled, Failed, Unknown`

`UDID`

`string`

 (Required) 

The unique identifier of the device.

`UserID`

`string`

For Shared iPad, this value is `FFFFFFFF-FFFF-FFFF-FFFF-FFFFFFFFFFFF` to indicate that authentication didn’t occur. In macOS, this value is the user identifier.

`UserLongName`

`string`

 (Required) 

The full name of the user.

`UserShortName`

`string`

For Shared iPad, this value is the Managed Apple ID of the user, which indicates the token is for the user channel. In macOS, this value is the short name of the user.

## Topics

### Commands

object InstallMediaResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object InstallMediaCommand

The command to install a book on a device.

