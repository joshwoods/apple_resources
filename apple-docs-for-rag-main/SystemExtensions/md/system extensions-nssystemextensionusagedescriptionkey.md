

- System Extensions
-  NSSystemExtensionUsageDescriptionKey 

Global Variable

# NSSystemExtensionUsageDescriptionKey

A message that tells the user why the app is trying to install a system extension bundle.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
let NSSystemExtensionUsageDescriptionKey: String
```

## Discussion

This key is required for all system extensions except DriverKit extensions, and must be in the extension’s `Info.plist` file. Failure to include this key results in an error at activation time. For DriverKit extensions, use OSBundleUsageDescriptionKey instead.

## See Also

### Usage descriptions

let OSBundleUsageDescriptionKey: String

A message that tells the user why the app is trying to install a driver extension bundle.

