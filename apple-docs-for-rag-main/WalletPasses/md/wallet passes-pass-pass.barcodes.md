

- Wallet Passes
- Pass
-  Pass.Barcodes 

Object

# Pass.Barcodes

An object that represents a barcode on a pass.

iOS 9.0+iPadOS 6.0+watchOS 2.0+

``` source
object Pass.Barcodes
```

## Properties

`altText`

`string`

The text to display near the barcode. For example, a human-readable version of the barcode data in case the barcode doesn’t scan.

The alternative text isn’t displayed for watchOS.

`format`

`string`

 (Required) 

The format of the barcode.

The barcode format PKBarcodeFormatCode128 isn’t supported for watchOS.

Possible Values: `PKBarcodeFormatQR, PKBarcodeFormatPDF417, PKBarcodeFormatAztec, PKBarcodeFormatCode128`

`message`

`string`

 (Required) 

The message or payload to display as a barcode.

`messageEncoding`

`string`

 (Required) 

The IANA character set name of the text encoding to use to convert `message` from a string representation to a data representation that the system renders as a barcode, such as `“iso-8859-1”`.

## See Also

### Adding barcodes

object Pass.Barcode

An object that represents a barcode shown on a pass.

Deprecated

