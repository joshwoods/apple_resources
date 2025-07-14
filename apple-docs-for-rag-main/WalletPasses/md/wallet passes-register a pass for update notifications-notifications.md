

- Wallet Passes
-  Register a Pass for Update Notifications 

Web Service Endpoint

# Register a Pass for Update Notifications

Set up change notifications for a pass on a device.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

## URL

``` source
POST https://yourpasshost.example.com/v1/devices/{deviceLibraryIdentifier}/registrations/{passTypeIdentifier}/{serialNumber}
```

## Path Parameters

`deviceLibraryIdentifier`

`string`

 (Required) 

A unique identifier you use to identify and authenticate the device.

`passTypeIdentifier`

`string`

 (Required) 

The pass type identifier of the pass to register for update notifications. This value corresponds to the value of the `passTypeIdentifier` key of the pass.

`serialNumber`

`string`

 (Required) 

The serial number of the pass to register. This value corresponds to the `serialNumber` key of the pass.

## Header Parameters

`Authorization`

`string`

The authentication for a pass. The value is the word `ApplePass`, followed by a space, followed by the `authenticationToken` key of the pass.

Value: `ApplePass {passAuthorizationToken}`

## HTTP Body

PushToken

An object that contains the push notification token for the registered pass on the device.

Content-Type: application/json

## Response Codes

` 200 ``Serial Number Already Registered for Device`

`Serial Number Already Registered for Device`

The serial number is already registered for the device.

` 201 ``Registration Successful`

`Registration Successful`

The registration is successful.

` 401 ``Request Not Authorized`

`Request Not Authorized`

The request isn’t authorized.

## See Also

### Pass Updates

Adding a Web Service to Update Passes

Implement a web server to register, update, and unregister a pass on a device.

Get the List of Updatable Passes

Send the serial numbers for updated passes to a device.

Send an Updated Pass

Create and sign an updated pass, and send it to the device.

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

