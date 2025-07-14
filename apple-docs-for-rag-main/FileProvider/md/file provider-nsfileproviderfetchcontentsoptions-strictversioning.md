

- File Provider
- NSFileProviderFetchContentsOptions
-  strictVersioning 

Type Property

# strictVersioning

An option that indicates the system requires an exact match of the requested item’s version.

macOS 12.3+

``` source
static var strictVersioning: NSFileProviderFetchContentsOptions { get }
```

## Discussion

If the system includes this option when calling your fetchPartialContents(for:version:request:minimalRange:aligningTo:options:completionHandler:) method, you must provide the requested version of the item. If you can’t provide the requested version, pass a NSFileProviderError.Code.versionNoLongerAvailable error to the completion handler instead.

