

- Core NFC
- NFCVASCommandConfiguration
-  passTypeIdentifier 

Instance Property

# passTypeIdentifier

A type identifier for the Wallet Pass.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var passTypeIdentifier: String { get set }
```

## Discussion

The reader session uses the string value to calculate the merchant ID value for the `GET VAS DATA` command.

## See Also

### Setting Configuration Items

var mode: NFCVASCommandConfiguration.Mode

A VAS protocol mode.

typealias VASMode

Constants that indicate the VAS protocol mode.

Deprecated

var url: URL?

A merchant URL.

