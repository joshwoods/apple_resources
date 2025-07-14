

- Foundation
- NSItemProviderWriting
-  writableTypeIdentifiersForItemProvider 

Type Property

# writableTypeIdentifiersForItemProvider

An array of UTI strings representing the types of data that can be loaded for an item provider.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
static var writableTypeIdentifiersForItemProvider: [String] { get }
```

**Required**

## Discussion

Provide uniform type identifiers (UTIs) in order from highest fidelity to lowest. If your app employs a native data representation, place that first in the array.

Implement this version of the property to offer a minimal list of UTIs that *all* resulting item provider instances can support. For example, using this version of the property for an NSURL object, your implementation should return the `public.url` UTI but not `public.file-url`.

Use the class version of this property when you do not initialize an item provider with an object, thereby deferring the underlying object’s instantiation until the destination app needs it.

## See Also

### Getting the writable type identifiers

var writableTypeIdentifiersForItemProvider: [String]

An array of UTI strings representing the types of data that can be loaded for an item provider.

