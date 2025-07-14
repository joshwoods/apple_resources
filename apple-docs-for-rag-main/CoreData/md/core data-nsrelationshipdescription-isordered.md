

- Core Data
- NSRelationshipDescription
-  isOrdered 

Instance Property

# isOrdered

A Boolean value that determines whether the relationship preserves the order of the referenced managed objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isOrdered: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Configuring the Destination

var inverseRelationship: NSRelationshipDescription?

The relationship that represents the inverse of the current relationship.

var destinationEntity: NSEntityDescription?

The type of object the relationship contains.

