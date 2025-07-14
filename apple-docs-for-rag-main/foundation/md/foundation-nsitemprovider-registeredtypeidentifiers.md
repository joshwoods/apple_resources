

- Foundation
- NSItemProvider
-  registeredTypeIdentifiers 

Instance Property

# registeredTypeIdentifiers

Returns the array of type identifiers for the item provider, in the same order they were registered.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var registeredTypeIdentifiers: [String] { get }
```

## See Also

### Querying the provider’s contents

func canLoadObject(ofClass: any NSItemProviderReading.Type) -> Bool

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

func canLoadObject&lt;T>(ofClass: T.Type) -> Bool

Returns a Boolean value indicating whether an item provider can load objects of a specified class.

func hasItemConformingToTypeIdentifier(String) -> Bool

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier file options parameter with a value of zero.

func hasRepresentationConforming(toTypeIdentifier: String, fileOptions: NSItemProviderFileOptions) -> Bool

Returns a Boolean value indicating whether an item provider contains a data representation conforming to a specified universal type identifier and to specified open-in-place behavior.

func registeredTypeIdentifiers(fileOptions: NSItemProviderFileOptions) -> [String]

Returns an array with a subset of type identifiers for the item provider, according to the specified file options, in the same order they were registered.

