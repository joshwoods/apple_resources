

- UIKit
-  UITrait 

Type Alias

# UITrait

A type representing a trait in a trait collection.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
typealias UITrait = any UITraitDefinition.Type
```

## Discussion

The type of a trait serves as a key to uniquely identify a trait in a trait collection. The subscript(_:) method of UITraitCollection and registerForTraitChanges(_:handler:) are two examples that take trait types to identify traits in the collection.

## See Also

### Custom traits

protocol UIMutableTraits

A mutable container of traits.

protocol UITraitDefinition

A type representing a trait in a trait collection.

