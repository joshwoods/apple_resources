

- Background Assets
- BADownloaderExtension
-  extensionWillTerminate() 

Instance Method

# extensionWillTerminate()

This method may be called shortly before the extension is terminated.

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac CatalystmacOS 13.0–13.3DeprecatedtvOS 18.4+visionOS 2.4–2.4Deprecated

``` source
func extensionWillTerminate()
```

**Required** Default implementation provided.

## Discussion

This method is invoked if all extension callbacks have returned or if the extension has run over it’s alotted runtime. This callback provides a last chance to tidy up state before process termination.

Warning

This method is advisory only, there will be instances where the extension is terminated before this method is invoked. Do not rely on this method being invoked before the extension is terminated.

## Default Implementations

### BADownloaderExtension Implementations

func extensionWillTerminate()

