

- Foundation
- NSKeyedUnarchiver
-  unarchivedDictionary(keysOfClasses:objectsOfClasses:from:) 

Type Method

# unarchivedDictionary(keysOfClasses:objectsOfClasses:from:)

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@nonobjc
static func unarchivedDictionary(
    keysOfClasses keyClasses: [AnyClass],
    objectsOfClasses objectClasses: [AnyClass],
    from data: Data
) throws -> [AnyHashable : Any]?
```

