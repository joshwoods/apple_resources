

- File Provider
- NSFileProviderManager
-  default 

Type Property

# default

A property that returns the shared file provider manager object.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
class var `default`: NSFileProviderManager { get }
```

## Discussion

This property returns a manager for the default domain on iOS. You can access the default domain in both the containing app and the File Provider extension. On macOS, use an explicit domain by calling init(for:) instead.

## See Also

### Accessing File Provider data

var documentStorageURL: URL

The root URL for all shared documents.

var providerIdentifier: String

A purpose identifier for coordinated reads and writes.

