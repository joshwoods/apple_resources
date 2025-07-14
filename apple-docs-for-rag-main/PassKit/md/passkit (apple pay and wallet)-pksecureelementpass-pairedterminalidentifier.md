

- PassKit (Apple Pay and Wallet)
- PKSecureElementPass
-  pairedTerminalIdentifier 

Instance Property

# pairedTerminalIdentifier

The unique identifier of the paired terminal.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var pairedTerminalIdentifier: String? { get }
```

## Discussion

PassKit can create a Secure Element pass during an exchange with a terminal. For example, when creating a digital car key. You can use this property’s value to identify the terminal.

## See Also

### Getting the hardware attributes

var deviceAccountIdentifier: String

The unique identifier for the device-specific account number.

var deviceAccountNumberSuffix: String

A display-ready version of the device-specific account number.

var devicePassIdentifier: String?

An opaque value for the pass.

