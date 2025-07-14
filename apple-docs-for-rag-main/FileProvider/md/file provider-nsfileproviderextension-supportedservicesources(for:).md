

- File Provider
- NSFileProviderExtension
-  supportedServiceSources(for:) 

Instance Method

# supportedServiceSources(for:)

Return an array of service sources that let the host app perform actions associated with the specified item.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

``` source
func supportedServiceSources(for itemIdentifier: NSFileProviderItemIdentifier) throws -> [any NSFileProviderServiceSource]
```

## See Also

### Working with services

protocol NSFileProviderServiceSource

A service that provides a custom communication channel between the host app and the File Provider extension.

