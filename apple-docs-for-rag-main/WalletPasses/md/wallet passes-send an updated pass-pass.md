

- Wallet Passes
-  Send an Updated Pass 

Web Service Endpoint

# Send an Updated Pass

Create and sign an updated pass, and send it to the device.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

## URL

``` source
GET https://yourpasshost.example.com/v1/passes/{passTypeIdentifier}/{serialNumber}
```

## Path Parameters

`passTypeIdentifier`

`string`

 (Required) 

The pass type identifier of the pass to update. This value corresponds to the value of the `passTypeIdentifier` key of the pass.

`serialNumber`

`string`

 (Required) 

The serial number of the pass to update. This value corresponds to the `serialNumber` key of the pass.

## Header Parameters

`Authorization`

`string`

The authentication for a pass. The value is the word `ApplePass`, followed by a space, followed by the `authenticationToken` key of the pass.

Value: `ApplePass {passAuthorizationToken}`

## Response Codes

` 200 ``OK`

`OK`

The request is successful and returns the updated pass.

Content-Type: application/vnd.apple.pkpass

` 401 ``Request Not Authorized`

`Request Not Authorized`

The request isn’t authorized.

## See Also

### Pass Updates

Adding a Web Service to Update Passes

Implement a web server to register, update, and unregister a pass on a device.

Register a Pass for Update Notifications

Set up change notifications for a pass on a device.

Get the List of Updatable Passes

Send the serial numbers for updated passes to a device.

Unregister a Pass for Update Notifications

Stop sending update notifications for a pass on a device.

Log a Message

Record a message on your server.

object PushToken

An object that contains the push notification token for a registered pass on a device.

object SerialNumbers

An object that contains serial numbers for the updatable passes on a device.

object LogEntries

An object that contains an array of messages.

