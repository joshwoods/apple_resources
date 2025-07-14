

- Foundation
- NSItemProvider
-  init() 

Initializer

# init()

Creates an empty item provider to which you can later register a data or file representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## See Also

### Creating an item provider

convenience init?(contentsOf: URL!)

Provides data-backed content from an existing file.

convenience init(contentsOf: URL, contentType: UTType?, openInPlace: Bool, coordinated: Bool, visibility: NSItemProviderRepresentationVisibility)

Provides data-backed content from an existing file with the specified parameters.

init(item: (any NSSecureCoding)?, typeIdentifier: String?)

Creates an item provider with an object, according to the item provider type coercion policy.

convenience init(object: any NSItemProviderWriting)

Creates a new item provider, employing a specified object’s type identifiers to specify the data representations eligible for the provider to load.

