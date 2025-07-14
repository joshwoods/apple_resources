

- Core Data
- NSRelationshipDescription
-  minCount 

Instance Property

# minCount

The minimum number of managed objects the relationship can reference.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var minCount: Int { get set }
```

## Discussion

If you declare a relationship attribute as optional when defining your entities, the framework only enforces minCount and maxCount when that attribute is not `nil`.

The default value is `0`.

## See Also

### Configuring Cardinality

var isToMany: Bool

Returns a Boolean value that indicates whether the relationship can contain many managed objects.

var maxCount: Int

The maximum number of managed objects the relationship can reference.

