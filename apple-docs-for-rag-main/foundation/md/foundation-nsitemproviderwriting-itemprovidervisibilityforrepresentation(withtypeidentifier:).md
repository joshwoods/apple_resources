

- Foundation
- NSItemProviderWriting
-  itemProviderVisibilityForRepresentation(withTypeIdentifier:) 

Type Method

# itemProviderVisibilityForRepresentation(withTypeIdentifier:)

Asks the item provider for the default representation visibility specification for the given UTI.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional static func itemProviderVisibilityForRepresentation(withTypeIdentifier typeIdentifier: String) -> NSItemProviderRepresentationVisibility
```

## Parameters 

`typeIdentifier`  

A uniform type identifier (UTI).

## Return Value

A representation visibility specification for the given UTI.

## See Also

### Getting the representation visibility specification

func itemProviderVisibilityForRepresentation(withTypeIdentifier: String) -> NSItemProviderRepresentationVisibility

Asks the item provider for the representation visibility specification for the given UTI.

