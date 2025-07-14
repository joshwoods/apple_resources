

- Device Management
- AirPrint
-  AirPrint.AirPrintItem 

Device Management Profile

# AirPrint.AirPrintItem

A dictionary of AirPrint printer details.

iOS 7.0+iPadOS 7.0+macOS 10.10+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object AirPrint.AirPrintItem
```

## Properties

`ForceTLS`

`boolean`

If `true`, AirPrint connections are secured by Transport Layer Security (TLS). Available only in iOS 11 and later.

Default: `false`

`IPAddress`

`string`

 (Required) 

The IP address or hostname of the AirPrint destination.

`Port`

`integer`

The listening port of the AirPrint destination. Available only in iOS 11 and later.

Minimum: `0`

Maximum: `65535`

`ResourcePath`

`string`

 (Required) 

The resource path associated with the printer. This path corresponds to the `rp` parameter of the `_ipps.tcp` Bonjour record. For example:

- `printers/Canon_MG5300_series`

- `printers/Xerox_Phaser_7600`

- `ipp/print`

- `Epson_IPP_Printer`

