

- Foundation
- NSItemProvider
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Provides data-backed content from an existing file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(contentsOf fileURL: URL!)
```

## Parameters 

`fileURL`  

The URL of the file to use for the item provider’s data. The item provider uses the filename extension to determine the universal type identifier for the associated data.

## Return Value

An item provider for the specified file, or `nil` if an error occurs.

## Discussion

The system uses the URL’s filename extension to select an appropriate universal type identifier. If the system can’t determine a specific universal type identifier based on the filename extension, it assigns the `public.data` universal type identifier for the file.

## See Also

### Related Documentation

App Extension Programming Guide

### Creating an item provider

convenience init(contentsOf: URL, contentType: UTType?, openInPlace: Bool, coordinated: Bool, visibility: NSItemProviderRepresentationVisibility)

Provides data-backed content from an existing file with the specified parameters.

init(item: (any NSSecureCoding)?, typeIdentifier: String?)

Creates an item provider with an object, according to the item provider type coercion policy.

init()

Creates an empty item provider to which you can later register a data or file representation.

convenience init(object: any NSItemProviderWriting)

Creates a new item provider, employing a specified object’s type identifiers to specify the data representations eligible for the provider to load.

