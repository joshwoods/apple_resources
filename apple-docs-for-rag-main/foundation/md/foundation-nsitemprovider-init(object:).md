

- Foundation
- NSItemProvider
-  init(object:) 

Initializer

# init(object:)

Creates a new item provider, employing a specified object’s type identifiers to specify the data representations eligible for the provider to load.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(object: any NSItemProviderWriting)
```

## Parameters 

`object`  

An object containing the data you want to provide.

## See Also

### Creating an item provider

convenience init?(contentsOf: URL!)

Provides data-backed content from an existing file.

convenience init(contentsOf: URL, contentType: UTType?, openInPlace: Bool, coordinated: Bool, visibility: NSItemProviderRepresentationVisibility)

Provides data-backed content from an existing file with the specified parameters.

init(item: (any NSSecureCoding)?, typeIdentifier: String?)

Creates an item provider with an object, according to the item provider type coercion policy.

init()

Creates an empty item provider to which you can later register a data or file representation.

