

- AVFoundation
- AVMetadataItem
-  key(forIdentifier:) 

Type Method

# key(forIdentifier:)

Returns a metadata key for the specified identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func key(forIdentifier identifier: AVMetadataIdentifier) -> Any?
```

## Parameters 

`identifier`  

The metadata identifier.

## Return Value

A metadata key.

## See Also

### Translating Metadata Items

class func identifier(forKey: Any, keySpace: AVMetadataKeySpace) -> AVMetadataIdentifier?

Returns a metadata identifier for the specified key and key space.

class func keySpace(forIdentifier: AVMetadataIdentifier) -> AVMetadataKeySpace?

Returns a metadata key space for the specified identifier.

