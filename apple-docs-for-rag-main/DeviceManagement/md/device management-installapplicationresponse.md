

- Device Management
-  InstallApplicationResponse 

Device Management Command

# InstallApplicationResponse

A response from the device after it processes the command to install a third-party app.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationResponse
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

`[`InstallApplicationResponse.ErrorChainItem`]`

An array of dictionaries that describes any errors that occurred.

`Identifier`

`string`

The app’s bundle identifier, if the user accepted the request.

Note

For a watchOS app, the identifier is the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired.

`NotOnConsole`

`boolean`

 (Required) 

If `true`, the device isn’t on-console.

`RejectionReason`

`string`

The reason, if installation fails.

Possible Values: `AppAlreadyInstalled, AppAlreadyQueued, AppStoreDisabled, CouldNotVerifyAppID, ManagementChangeNotSupported, NotAnApp, NotSupported, Other, PurchaseMethodNotSupported, PurchaseMethodNotSupportedInMultiUser`

`State`

`string`

The app’s installation state, if the user accepted the request. If this value is `NeedsRedemption`, the server must send a redemption code to complete the app installation.

Possible Values: `Queued, NeedsRedemption, Redeeming, Prompting, PromptingForLogin, ValidatingPurchase, Installing, Managed, ManagedButUninstalled, UserInstalledApp, UserRejected, PromptingForUpdate, PromptingForUpdateLogin, ValidatingUpdate, Updating, UpdateRejected, PromptingForManagement, ManagementRejected, Failed, Unknown`

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

object InstallApplicationResponse.ErrorChainItem

A dictionary that describes an error chain item.

## See Also

### Command and Response

object InstallApplicationCommand

The command to install an app on a device.

