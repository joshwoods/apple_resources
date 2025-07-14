

- Wallet Passes
- Pass
-  Pass.Barcode Deprecated

Object

# Pass.Barcode

An object that represents a barcode shown on a pass.

iOS 6.0–9.0DeprecatediPadOS 6.0+watchOS 2.0+

``` source
object Pass.Barcode
```

Deprecated

Use Pass.Barcodes instead.

## Properties

`altText`

`string`

The text displayed near the barcode. For example, a human-readable version of the barcode data in case the barcode doesn’t scan.

The alternative text isn’t displayed for watchOS.

`format`

`string`

 (Required) 

The format of the barcode.

The barcode format PKBarcodeFormatCode128 isn’t supported for watchOS.

Possible Values: `PKBarcodeFormatQR, PKBarcodeFormatPDF417, PKBarcodeFormatAztec`

`message`

`string`

 (Required) 

The message or payload to display as a barcode.

`messageEncoding`

`string`

 (Required) 

The IANA character set name of the text encoding to use to convert `message` from a string representation to a data representation that the system renders as a barcode, such as `“iso-8859-1”`

## See Also

### Adding barcodes

object Pass.Barcodes

An object that represents a barcode on a pass.

