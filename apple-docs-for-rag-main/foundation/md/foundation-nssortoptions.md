

- Foundation
-  NSSortOptions 

Structure

# NSSortOptions

Options for block sorting operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSSortOptions
```

## Topics

### Constants

static var concurrent: NSSortOptions

Specifies that the Block sort operation should be concurrent.

static var stable: NSSortOptions

Specifies that the sorted results should return compared items having equal value in the order they occurred originally.

### Initializers

init(rawValue: UInt)

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

### Iteration

class NSEnumerator

An abstract class whose subclasses enumerate collections of objects, such as arrays and dictionaries.

protocol NSFastEnumeration

A protocol that objects adopt to support fast enumeration.

struct NSFastEnumerationIterator

struct NSIndexSetIterator

An iterator suitable for enumerating the elements of an index set.

struct NSEnumerationOptions

Options for block enumeration operations.

