

- Device Management
- Printing
- Printing.UserPrinterList
-  Printing.UserPrinterList.Printer 

Device Management Profile

# Printing.UserPrinterList.Printer

A printer dictionary.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Printing.UserPrinterList.Printer
```

## Properties

`DeviceURI`

`string`

The device URI.

`DisplayName`

`string`

The display name.

`Location`

`string`

The printer’s location.

`Model`

`string`

The printer’s model.

`PPDURL`

`string`

The printer’s PPDURL.

`PrinterLocked`

`boolean`

If `true`, locks the printer.

Default: `false`

## See Also

### Objects

object Printing.DefaultPrinter

A default printer for the user.

object Printing.UserPrinterList

A list of printer dictionaries.

