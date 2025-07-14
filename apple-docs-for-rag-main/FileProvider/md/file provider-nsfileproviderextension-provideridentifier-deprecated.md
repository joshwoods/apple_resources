

- File Provider
- NSFileProviderExtension
-  providerIdentifier Deprecated

Instance Property

# providerIdentifier

A purpose identifier for coordinated reads and writes.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var providerIdentifier: String { get }
```

Deprecated

Use the NSFileProviderManager class’s providerIdentifier method instead.

## Discussion

This property contains a unique string that can be used as a purpose identifier for file coordination. The File Provider extension should use this identifier when performing coordinated reads and writes, to help prevent deadlocks.

Pass this identifier to the file coordinator’s `setPurposeIdentifier:` method before performing a coordinated read or write.

This method returns the containing app’s bundle identifier.

## See Also

### Accessing the document storage

var documentStorageURL: URL

The root URL for all shared documents.

Deprecated

