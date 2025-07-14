

- UIKit
- UIPasteConfiguration
-  addTypeIdentifiers(forAccepting:) 

Instance Method

# addTypeIdentifiers(forAccepting:)

Expands the array of accepted UTIs for a paste configuration, based on those declared as supported by a specified class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addTypeIdentifiers(forAccepting aClass: any NSItemProviderReading.Type)
```

## Parameters 

`aClass`  

A class conforming to the NSItemProviderReading protocol.

## Discussion

This method uses the property readableTypeIdentifiersForItemProvider, implemented on `aClass`, to determine the uniform type identifiers (UTIs) to add to the paste configuration’s acceptableTypeIdentifiers array.

## See Also

### Adding acceptable type identifiers

func addAcceptableTypeIdentifiers([String])

Adds an array of UTI strings to a paste configuration, increasing the variety of types the paste configuration accepts.

func addTypeIdentifiers&lt;T>(forAccepting: T.Type)

