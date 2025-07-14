

- Foundation
- NSItemProvider
-  init(contentsOf:contentType:openInPlace:coordinated:visibility:) 

Initializer

# init(contentsOf:contentType:openInPlace:coordinated:visibility:)

Provides data-backed content from an existing file with the specified parameters.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    contentsOf fileURL: URL,
    contentType: UTType?,
    openInPlace: Bool = false,
    coordinated: Bool = false,
    visibility: NSItemProviderRepresentationVisibility = .all
)
```

## Parameters 

`fileURL`  

The URL of the file to use for the item provider’s data.

`contentType`  

The content type of the specified file.

`openInPlace`  

`true` if the system opens the file in place.

`coordinated`  

`true` if the returned file must be accessed using NSFileCoordinator.

`visibility`  

The NSItemProviderRepresentationVisibility setting the system uses to identify which processes can see this content.

## Discussion

If openInPlace is set to `false`, the system copies the file provided before the load handler returns.

## See Also

### Creating an item provider

convenience init?(contentsOf: URL!)

Provides data-backed content from an existing file.

init(item: (any NSSecureCoding)?, typeIdentifier: String?)

Creates an item provider with an object, according to the item provider type coercion policy.

init()

Creates an empty item provider to which you can later register a data or file representation.

convenience init(object: any NSItemProviderWriting)

Creates a new item provider, employing a specified object’s type identifiers to specify the data representations eligible for the provider to load.

