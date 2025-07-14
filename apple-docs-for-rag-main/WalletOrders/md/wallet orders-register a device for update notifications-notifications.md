

- Wallet Orders
-  Register a device for update notifications 

Web Service Endpoint

# Register a device for update notifications

Registers a device to receive update notifications for an order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

## URL

``` source
POST https://your-web-service.com/v1/devices/{deviceIdentifier}/registrations/{orderTypeIdentifier}/{orderIdentifier}
```

## Path Parameters

`orderIdentifier`

`string`

 (Required) 

The order identifier. This value corresponds to the value of the `orderIdentifier` key of the Order.

`orderTypeIdentifier`

`string`

 (Required) 

The order type identifier of the order. This value corresponds to the value of the `orderTypeIdentifier` key of the Order.

`deviceIdentifier`

`string`

 (Required) 

A unique identifier for the device.

## Header Parameters

`Authorization`

`string`

 (Required) 

The authentication for an order. The scheme is `AppleOrder` with the order’s value for the `authenticationToken` key as parameter. For example, `AppleOrder {authenticationToken}`.

Value: `AppleOrder {authenticationToken}`

## HTTP Body

PushToken

The push token APNS uses to send update notifications to the device.

Content-Type: application/json

## Response Codes

` 200 ``Device Already Registered`

`Device Already Registered`

The device is already registered for the order.

` 201 ``Device Registered`

`Device Registered`

The device successfully registered for the order.

` 401 ``Request Not Authorized`

`Request Not Authorized`

The request isn’t authorized.

## Discussion

When the system modifies an order, use the PushToken to send a push notification to the device. In the notification, set the push topic as the order type identifier and leave the payload empty.

## See Also

### Notifications

Unregister a device from update notifications

Unregisters a device from receiving update notifications for an order.

object PushToken

The push token APNS uses to send update notifications to the device.

