

- Foundation
- NSCoder
-  decodeDictionary(withKeyClass:objectClass:forKey:) 

Instance Method

# decodeDictionary(withKeyClass:objectClass:forKey:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
func decodeDictionary(
    withKeyClass keyClass: DecodedKey.Type,
    objectClass: DecodedObject.Type,
    forKey key: String
) -> [DecodedKey : DecodedObject]? where DecodedKey : NSObject, DecodedKey : NSCopying, DecodedKey : NSSecureCoding, DecodedObject : NSObject, DecodedObject : NSSecureCoding
```

