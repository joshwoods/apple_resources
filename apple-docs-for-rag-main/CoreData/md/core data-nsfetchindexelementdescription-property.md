

- Core Data
- NSFetchIndexElementDescription
-  property 

Instance Property

# property

A property description.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var property: NSPropertyDescription? { get }
```

## Discussion

This property may also be an NSExpressionDescription that expresses a function.

## See Also

### Inspecting an Index Element Description

var collationType: NSFetchIndexElementType

The type of collation that the index element uses, either binary or R-tree.

var indexDescription: NSFetchIndexDescription?

var isAscending: Bool

A Boolean value that controls whether an index that supports direction is an ascending or descending index.

var propertyName: String?

The specified name in the property description.

