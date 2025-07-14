

- Wallet Orders
-  Unregister a device from update notifications 

Web Service Endpoint

# Unregister a device from update notifications

Unregisters a device from receiving update notifications for an order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

## URL

``` source
DELETE https://your-web-service.com/v1/devices/{deviceIdentifier}/registrations/{orderTypeIdentifier}/{orderIdentifier}
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

## Response Codes

` 200 ``Device Unregistered`

`Device Unregistered`

The device successfully unregistered.

` 401 ``Request Not Authorized`

`Request Not Authorized`

The request isn’t authorized.

## See Also

### Notifications

Register a device for update notifications

Registers a device to receive update notifications for an order.

object PushToken

The push token APNS uses to send update notifications to the device.

