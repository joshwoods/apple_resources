

- Wallet Passes
-  Get the List of Updatable Passes 

Web Service Endpoint

# Get the List of Updatable Passes

Send the serial numbers for updated passes to a device.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

## URL

``` source
GET https://yourpasshost.example.com/v1/devices/{deviceLibraryIdentifier}/registrations/{passTypeIdentifier}?passesUpdatedSince={previousLastUpdated}
```

## Path Parameters

`deviceLibraryIdentifier`

`string`

 (Required) 

The unique identifier for the device.

`passTypeIdentifier`

`string`

 (Required) 

The pass type identifier of the pass to check for updates. This value corresponds to the value of the `passTypeIdentifier` key of the pass.

`previousLastUpdated`

`string`

 (Required) 

The value of the `lastUpdated` key from the SerialNumbers object returned in a previous request. This value limits the results of the current request to the passes updated since that previous request.

## Response Codes

` 200 ``Return Matching Passes`

SerialNumbers

`Return Matching Passes`

On success, the call returns an object that contains the serial numbers for the matching passes.

Content-Type: application/json

` 204 ``No Matching Passes`

`No Matching Passes`

There are no matching passes.

## Mentioned in 

Adding a Web Service to Update Passes

## See Also

### Pass Updates

Adding a Web Service to Update Passes

Implement a web server to register, update, and unregister a pass on a device.

Register a Pass for Update Notifications

Set up change notifications for a pass on a device.

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

