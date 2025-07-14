

- Foundation
- NSOrderedCollectionDifferenceCalculationOptions
-  inferMoves 

Type Property

# inferMoves

An option that identifies insertions or removals as moves.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var inferMoves: NSOrderedCollectionDifferenceCalculationOptions { get }
```

## Discussion

When you use the option to infer moves, the difference calculation adds an associated index to change objects to indicate the original positions of the objects.

## See Also

### Difference Calculation Options

static var omitInsertedObjects: NSOrderedCollectionDifferenceCalculationOptions

An option that indicates that the difference should omit references to the insertions.

static var omitRemovedObjects: NSOrderedCollectionDifferenceCalculationOptions

An option that indicates that the difference should omit references to the removals.

