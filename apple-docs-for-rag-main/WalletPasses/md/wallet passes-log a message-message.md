

- Wallet Passes
-  Log a Message 

Web Service Endpoint

# Log a Message

Record a message on your server.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

## URL

``` source
POST https://yourpasshost.example.com/v1/log
```

## HTTP Body

LogEntries

An object that contains an array of messages.

Content-Type: application/json

## Response Codes

` 200 ``OK`

`OK`

The request is successful.

## See Also

### Pass Updates

Adding a Web Service to Update Passes

Implement a web server to register, update, and unregister a pass on a device.

Register a Pass for Update Notifications

Set up change notifications for a pass on a device.

Get the List of Updatable Passes

Send the serial numbers for updated passes to a device.

Send an Updated Pass

Create and sign an updated pass, and send it to the device.

Unregister a Pass for Update Notifications

Stop sending update notifications for a pass on a device.

object PushToken

An object that contains the push notification token for a registered pass on a device.

object SerialNumbers

An object that contains serial numbers for the updatable passes on a device.

object LogEntries

An object that contains an array of messages.

