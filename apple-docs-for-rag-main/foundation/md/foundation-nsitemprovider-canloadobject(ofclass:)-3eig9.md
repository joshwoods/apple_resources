

- Foundation
- NSItemProvider
-  canLoadObject(ofClass:) 

Instance Method

# canLoadObject(ofClass:)

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func canLoadObject(ofClass aClass: any NSItemProviderReading.Type) -> Bool
```

## Parameters 

`aClass`  

The object class for comparison.

## Return Value

`true` if the item provider can load objects of the class.

## See Also

### Querying the provider’s contents

func canLoadObject&lt;T>(ofClass: T.Type) -> Bool

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

func hasItemConformingToTypeIdentifier(String) -> Bool

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier file options parameter with a value of zero.

func hasRepresentationConforming(toTypeIdentifier: String, fileOptions: NSItemProviderFileOptions) -> Bool

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier and to specified open-in-place behavior.

var registeredTypeIdentifiers: [String]

Returns the array of type identifiers for the item provider, in the same order they were registered.

func registeredTypeIdentifiers(fileOptions: NSItemProviderFileOptions) -> [String]

Returns an array with a subset of type identifiers for the item provider, according to the specified file options, in the same order they were registered.

