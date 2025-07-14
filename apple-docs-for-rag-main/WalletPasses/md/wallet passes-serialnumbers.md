

- Wallet Passes
-  SerialNumbers 

Object

# SerialNumbers

An object that contains serial numbers for the updatable passes on a device.

iOS 6.0+iPadOS 6.0+watchOS 2.0+

``` source
object SerialNumbers
```

## Properties

`serialNumbers`

`[string]`

An array of serial numbers for the updated passes.

`lastUpdated`

`string`

A developer-defined string that contains a tag that indicates the modification time for the returned passes.

You use the value of this key for the `previousLastUpdated` parameter of Get the List of Updatable Passes to return passes modified after the represented date and time.

## Mentioned in 

Adding a Web Service to Update Passes

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

Log a Message

Record a message on your server.

object PushToken

An object that contains the push notification token for a registered pass on a device.

object LogEntries

An object that contains an array of messages.

