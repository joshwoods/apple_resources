

- Foundation
- NSItemProvider
-  hasItemConformingToTypeIdentifier(\_:) 

Instance Method

# hasItemConformingToTypeIdentifier(\_:)

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier file options parameter with a value of zero.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func hasItemConformingToTypeIdentifier(_ typeIdentifier: String) -> Bool
```

## Parameters 

`typeIdentifier`  

A string that represents the desired UTI.

## See Also

### Querying the provider’s contents

func canLoadObject(ofClass: any NSItemProviderReading.Type) -> Bool

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

func canLoadObject&lt;T>(ofClass: T.Type) -> Bool

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

func hasRepresentationConforming(toTypeIdentifier: String, fileOptions: NSItemProviderFileOptions) -> Bool

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier and to specified open-in-place behavior.

var registeredTypeIdentifiers: [String]

Returns the array of type identifiers for the item provider, in the same order they were registered.

func registeredTypeIdentifiers(fileOptions: NSItemProviderFileOptions) -> [String]

Returns an array with a subset of type identifiers for the item provider, according to the specified file options, in the same order they were registered.

