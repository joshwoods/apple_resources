

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  deviceAccountNumberSuffix 

Instance Property

# deviceAccountNumberSuffix

A display-ready version of the device-specific account number.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var deviceAccountNumberSuffix: String { get }
```

## Discussion

This property’s value is generally the last four or five digits of the device-specific account number, but can vary by issuer.

## See Also

### Getting the hardware attributes

var deviceAccountIdentifier: String

The unique identifier for the device-specific account number.

var devicePassIdentifier: String?

An opaque value for the pass.

var pairedTerminalIdentifier: String?

The unique identifier of the paired terminal.

