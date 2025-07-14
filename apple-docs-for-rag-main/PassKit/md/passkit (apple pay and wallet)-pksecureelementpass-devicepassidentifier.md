

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  devicePassIdentifier 

Instance Property

# devicePassIdentifier

An opaque value for the pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var devicePassIdentifier: String? { get }
```

## Discussion

Important

This property’s value is unique for each issuer. This property is available only to developers who work with Apple to enable this functionality.

## See Also

### Getting the hardware attributes

var deviceAccountIdentifier: String

The unique identifier for the device-specific account number.

var deviceAccountNumberSuffix: String

A display-ready version of the device-specific account number.

var pairedTerminalIdentifier: String?

The unique identifier of the paired terminal.

