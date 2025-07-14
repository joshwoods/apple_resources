

- Foundation
-  NSOrderedCollectionDifferenceCalculationOptions 

Structure

# NSOrderedCollectionDifferenceCalculationOptions

Constants that specify the options to use when creating an ordered collection difference.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct NSOrderedCollectionDifferenceCalculationOptions
```

## Topics

### Creating Difference Calculation Options

init(rawValue: UInt)

### Difference Calculation Options

static var inferMoves: NSOrderedCollectionDifferenceCalculationOptions

An option that identifies insertions or removals as moves.

static var omitInsertedObjects: NSOrderedCollectionDifferenceCalculationOptions

An option that indicates that the difference should omit references to the insertions.

static var omitRemovedObjects: NSOrderedCollectionDifferenceCalculationOptions

An option that indicates that the difference should omit references to the removals.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Comparing with Another Array

class NSOrderedCollectionDifference

An object representing the difference between two ordered collections.

