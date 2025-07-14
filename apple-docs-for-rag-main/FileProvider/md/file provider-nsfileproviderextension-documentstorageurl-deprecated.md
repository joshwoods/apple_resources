

- File Provider
- NSFileProviderExtension
-  documentStorageURL Deprecated

Instance Property

# documentStorageURL

The root URL for all shared documents.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var documentStorageURL: URL { get }
```

Deprecated

Use the NSFileProviderManager class’s documentStorageURL method instead.

## Discussion

This property contains the URL `/File Provider Storage`, where *container URL* is the value returned by the containerURL(forSecurityApplicationGroupIdentifier:) method.

The container URL refers to an app group container directory used by the `NSFileProviderExtension` extension. You can specify this shared container using the `NSExtensionFileProviderDocumentGroup` key in the File Provider extension’s `info.plist` file.

## See Also

### Accessing the document storage

var providerIdentifier: String

A purpose identifier for coordinated reads and writes.

Deprecated

