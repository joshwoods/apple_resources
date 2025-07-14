

- Foundation
- NSItemProvider
-  init(item:typeIdentifier:) 

Initializer

# init(item:typeIdentifier:)

Creates an item provider with an object, according to the item provider type coercion policy.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    item: (any NSSecureCoding)?,
    typeIdentifier: String?
)
```

## Parameters 

`item`  

An object containing the data you want to provide. You may specify `nil` for this parameter and register items and types later.

`typeIdentifier`  

A string that represents the UTI of the item. If `item` is not `nil`, this parameter must not be `nil`.

## Return Value

An item provider for the specified item.

## Discussion

Use this method to initialize an item provider for objects in your app. The item provider registers your object with the specified type. Subsequent requests for that same type return the specified `item`.

## See Also

### Creating an item provider

convenience init?(contentsOf: URL!)

Provides data-backed content from an existing file.

convenience init(contentsOf: URL, contentType: UTType?, openInPlace: Bool, coordinated: Bool, visibility: NSItemProviderRepresentationVisibility)

Provides data-backed content from an existing file with the specified parameters.

init()

Creates an empty item provider to which you can later register a data or file representation.

convenience init(object: any NSItemProviderWriting)

Creates a new item provider, employing a specified object’s type identifiers to specify the data representations eligible for the provider to load.

