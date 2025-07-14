

- System Extensions
-  OSBundleUsageDescriptionKey 

Global Variable

# OSBundleUsageDescriptionKey

A message that tells the user why the app is trying to install a driver extension bundle.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
let OSBundleUsageDescriptionKey: String
```

## Discussion

This key is required for all DriverKit extensions and must be in the extension’s `Info.plist` file. Failure to include this key results in an error at activation time. For system extensions that are not DriverKit extensions, use NSSystemExtensionUsageDescriptionKey instead.

## See Also

### Usage descriptions

let NSSystemExtensionUsageDescriptionKey: String

A message that tells the user why the app is trying to install a system extension bundle.

