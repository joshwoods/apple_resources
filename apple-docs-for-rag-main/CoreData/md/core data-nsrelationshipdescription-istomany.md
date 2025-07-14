

- Core Data
- NSRelationshipDescription
-  isToMany 

Instance Property

# isToMany

Returns a Boolean value that indicates whether the relationship can contain many managed objects.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var isToMany: Bool { get }
```

## Discussion

If maxCount is equal to `1`, implying a to-one relationship, this property returns false; otherwise, it returns true.

## See Also

### Configuring Cardinality

var minCount: Int

The minimum number of managed objects the relationship can reference.

var maxCount: Int

The maximum number of managed objects the relationship can reference.

