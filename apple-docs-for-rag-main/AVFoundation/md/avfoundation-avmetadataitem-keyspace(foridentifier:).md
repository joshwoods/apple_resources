

- AVFoundation
- AVMetadataItem
-  keySpace(forIdentifier:) 

Type Method

# keySpace(forIdentifier:)

Returns a metadata key space for the specified identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func keySpace(forIdentifier identifier: AVMetadataIdentifier) -> AVMetadataKeySpace?
```

## Parameters 

`identifier`  

The metadata identifier.

## Return Value

A metadata key space.

## See Also

### Translating Metadata Items

class func identifier(forKey: Any, keySpace: AVMetadataKeySpace) -> AVMetadataIdentifier?

Returns a metadata identifier for the specified key and key space.

class func key(forIdentifier: AVMetadataIdentifier) -> Any?

Returns a metadata key for the specified identifier.

