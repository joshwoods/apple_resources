

- Core NFC
- NFCVASCommandConfiguration
-  url 

Instance Property

# url

A merchant URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var url: URL? { get set }
```

## Discussion

The maximum length of the URL is 64 characters, including the schema. To disable the merchant URL, set url to `nil.`

## See Also

### Setting Configuration Items

var mode: NFCVASCommandConfiguration.Mode

A VAS protocol mode.

typealias VASMode

Constants that indicate the VAS protocol mode.

Deprecated

var passTypeIdentifier: String

A type identifier for the Wallet Pass.

