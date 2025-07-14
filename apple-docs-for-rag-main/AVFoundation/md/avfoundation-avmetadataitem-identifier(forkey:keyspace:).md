

- AVFoundation
- AVMetadataItem
-  identifier(forKey:keySpace:) 

Type Method

# identifier(forKey:keySpace:)

Returns a metadata identifier for the specified key and key space.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func identifier(
    forKey key: Any,
    keySpace: AVMetadataKeySpace
) -> AVMetadataIdentifier?
```

## Parameters 

`key`  

A key to return an identifier for.

`keySpace`  

A key space to return an identifier for.

## Return Value

A metadata identifier, or `nil` if no equivalent identifier exists.

## See Also

### Translating Metadata Items

class func key(forIdentifier: AVMetadataIdentifier) -> Any?

Returns a metadata key for the specified identifier.

class func keySpace(forIdentifier: AVMetadataIdentifier) -> AVMetadataKeySpace?

Returns a metadata key space for the specified identifier.

