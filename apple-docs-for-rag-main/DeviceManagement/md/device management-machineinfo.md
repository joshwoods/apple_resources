

- Device Management
-  MachineInfo 

Object

# MachineInfo

A device’s information in response to a MDM enrollment profile request.

iOS 7.0+iPadOS 7.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object MachineInfo
```

## Properties

`IMEI`

`string`

The device’s IMEI (if available).

`LANGUAGE`

`string`

The user’s currently-selected language, for example, `en`.

`MDM_CAN_REQUEST_SOFTWARE_UPDATE`

`boolean`

If `true`, indicates that the server can trigger the device to do a required software update.

Available on iOS 17 and later, and macOS 14 and later.

Default: `false`

`MEID`

`string`

The device’s MEID (if available).

`OS_VERSION`

`string`

 (Required) 

The OS version installed on the device, for example, 17.0.

Available on iOS 17 and later, macOS 14 and later, tvOS 17 and later, and watchOS 10 and later.

`PAIRING_TOKEN`

`data`

The pairing token to validate when a watch is enrolling.

Available on watchOS 10 and later.

`PRODUCT`

`string`

 (Required) 

The device’s product type, for example, `iPhone5,1`.

`SERIAL`

`string`

 (Required) 

The device’s serial number.

`SOFTWARE_UPDATE_DEVICE_ID`

`string`

The device model identifier used to lookup available OS updates through https://gdmf.apple.com/v2/pmv. Available on iOS 17.4 and later, macOS 14.4 and later, and visionOS 1.1 and later.

`SUPPLEMENTAL_BUILD_VERSION`

`string`

The device’s operating system supplemental build version (if available).

Available on iOS 17 and later, macOS 14 and later, tvOS 17 and later, and watchOS 10 and later.

`SUPPLEMENTAL_OS_VERSION_EXTRA`

`string`

The device’s operating system supplemental OS version extra (if available).

Available on iOS 17 and later, macOS 14 and later, tvOS 17 and later, and watchOS 10 and later.

`UDID`

`string`

 (Required) 

The device’s UDID.

`VERSION`

`string`

 (Required) 

The OS version installed on the device, for example, `7A182`.

## Discussion

This dictionary is CMS-signed with the device identity certificate. The system includes the device’s certificate and all necessary intermediate certificates. The certificate chain should validate against the Apple Root CA.

## See Also

### Objects and Data Types

object Device

A device’s properties and their values.

object Profile

A profile’s properties and their values.

object Limit

A ranged limit.

object Url

A URL object.

