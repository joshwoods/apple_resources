

- Device Management
-  AuthenticateRequest 

Device Management Command

# AuthenticateRequest

The Authenticate Request details.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AuthenticateRequest
```

## Properties

`BuildVersion`

`string`

The device’s build version.

`DeviceName`

`string`

 (Required) 

The device’s name.

`EnrollmentID`

`string`

The per-enrollment identifier for the device. The system requires this value if the enrollment type is user enrollment.

Available in macOS 10.15 and iOS 13.0 and later.

`IMEI`

`string`

The device’s IMEI (International Mobile Station Equipment Identity).

`MEID`

`string`

The device’s MEID (Mobile Equipment Identifier).

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `Authenticate`.

Value: `Authenticate`

`Model`

`string`

 (Required) 

The device’s model.

`ModelName`

`string`

 (Required) 

The device’s model name.

`OSVersion`

`string`

The device’s OS version.

`ProductName`

`string`

The device’s product name (`iPhone3,1`).

`SerialNumber`

`string`

The device’s serial number.

`Topic`

`string`

 (Required) 

The topic to which the device subscribes.

`UDID`

`string`

The device’s UDID (Unique Device ID). The system requires this value if the enrollment type isn’t user enrollment.

