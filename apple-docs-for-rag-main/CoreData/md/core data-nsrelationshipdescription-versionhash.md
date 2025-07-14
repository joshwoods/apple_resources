

- Core Data
- NSRelationshipDescription
-  versionHash 

Instance Property

# versionHash

The relationship’s unique identity.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var versionHash: Data { get }
```

## Discussion

To calculate its version hash, the relationship combines its superclass’s versionHash property with the values of inverseRelationship, destinationEntity, minCount, and maxCount.

