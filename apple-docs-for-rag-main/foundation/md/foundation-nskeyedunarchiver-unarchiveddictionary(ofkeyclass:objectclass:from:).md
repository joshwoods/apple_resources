

- Foundation
- NSKeyedUnarchiver
-  unarchivedDictionary(ofKeyClass:objectClass:from:) 

Type Method

# unarchivedDictionary(ofKeyClass:objectClass:from:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
static func unarchivedDictionary(
    ofKeyClass keyClass: DecodedKey.Type,
    objectClass: DecodedObject.Type,
    from data: Data
) throws -> [DecodedKey : DecodedObject]? where DecodedKey : NSObject, DecodedKey : NSCopying, DecodedKey : NSSecureCoding, DecodedObject : NSObject, DecodedObject : NSSecureCoding
```

