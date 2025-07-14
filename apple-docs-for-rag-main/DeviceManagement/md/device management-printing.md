

- Device Management
-  Printing 

Device Management Profile

# Printing

The payload you use to configure printers.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Printing
```

## Properties

`AllowLocalPrinters`

`boolean`

If `true`, allows printers that connect directly to a user’s computer.

Default: `true`

`DefaultPrinter`

Printing.DefaultPrinter

The default printer for the user.

`FooterFontName`

`string`

The footer font name.

`FooterFontSize`

`string`

The footer font size.

`PrintFooter`

`boolean`

If `true`, prints the page footer (including the user name and date).

Default: `false`

`PrintMACAddress`

`boolean`

If `true`, includes the MAC address.

Default: `false`

`RequireAdminToAddPrinters`

`boolean`

If `true`, requires an administrator password to add printers.

Default: `true`

`RequireAdminToPrintLocally`

`boolean`

If `true`, requires an administrator password to print locally.

Default: `false`

`ShowOnlyManagedPrinters`

`boolean`

If `true`, shows only managed printers.

Default: `false`

`UserPrinterList`

Printing.UserPrinterList

The printers available to a user.

## Discussion

Specify `com.apple.mcxprinting` as the payload type.

Removing this profile from a device does not automatically remove printers from the device.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            RequireAdminToAddPrinters

            AllowLocalPrinters

            RequireAdminToPrintLocally

            ShowOnlyManagedPrinters

            PrintFooter

            PrintMACAddress

            FooterFontSize
            7
            FooterFontName
            Helvetica
            DefaultPrinter

                DeviceURI
                ipp://printer.example.com/
                DisplayName
                printer.example.com

            UserPrinterList

                printer_example_com

                    DeviceURI
                    ipp://printer.example.com/
                    DisplayName
                    printer.example.com
                    Location
                    My Office
                    Model
                    PrinterModel1
                    PrinterLocked

                    PPDURL
                    file://localhost/System/Library/Frameworks/ApplicationServices.framework/Versions/A/Frameworks/PrintCore.framework/Resources/Generic.ppd

            PayloadIdentifier
            com.example.myprinterpayload
            PayloadType
            com.apple.mcxprinting
            PayloadUUID
            8242d870-95c0-0135-0b44-0c4de9ce4c04
            PayloadVersion
            1

    PayloadDisplayName
    Printing
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    ab59f143-1478-419a-885e-7994fb13c9c3
    PayloadVersion
    1

```

## Topics

### Objects

object Printing.DefaultPrinter

A default printer for the user.

object Printing.UserPrinterList

A list of printer dictionaries.

object Printing.UserPrinterList.Printer

A printer dictionary.

## See Also

### Printing

object AirPrint

The payload you use to configure AirPrint printers in the user’s printer list.

