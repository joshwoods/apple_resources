

- Core Data
- NSRelationshipDescription
-  destinationEntity 

Instance Property

# destinationEntity

The type of object the relationship contains.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var destinationEntity: NSEntityDescription? { get set }
```

## See Also

### Configuring the Destination

var inverseRelationship: NSRelationshipDescription?

The relationship that represents the inverse of the current relationship.

var isOrdered: Bool

A Boolean value that determines whether the relationship preserves the order of the referenced managed objects.

