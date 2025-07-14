

- File Provider
- NSFileProviderManager
-  documentStorageURL 

Instance Property

# documentStorageURL

The root URL for all shared documents.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
var documentStorageURL: URL { get }
```

## Discussion

This property contains the URL `/File Provider Storage`, where *container URL* is the value returned by the containerURL(forSecurityApplicationGroupIdentifier:) method.

The container URL refers to an app group container directory used by the `NSFileProviderExtension` extension. You can specify this shared container using the `NSExtensionFileProviderDocumentGroup` key in the File Provider extension’s `info.plist` file.

Note

While this property is available on macOS 11+, you don’t need to use it when creating a file provider extension that adopts the NSFileProviderReplicatedExtension protocol.

## See Also

### Accessing File Provider data

class var `default`: NSFileProviderManager

A property that returns the shared file provider manager object.

var providerIdentifier: String

A purpose identifier for coordinated reads and writes.

