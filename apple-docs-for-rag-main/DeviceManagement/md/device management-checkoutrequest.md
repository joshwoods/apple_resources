

- Device Management
-  CheckOutRequest 

Device Management Command

# CheckOutRequest

The Check Out Request details.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object CheckOutRequest
```

## Properties

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `CheckOut`.

Value: `CheckOut`

`Topic`

`string`

 (Required) 

The topic to which the device subscribed.

`UDID`

`string`

 (Required) 

The device’s UDID (Unique Device ID).

`EnrollmentID`

`string`

 (Required) 

The per-enrollment identifier for the device. Available in macOS 10.15 and iOS 13.0 and later.

