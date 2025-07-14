

- Foundation
-  NSEnumerationOptions 

Structure

# NSEnumerationOptions

Options for block enumeration operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct NSEnumerationOptions
```

## Topics

### Constants

static var concurrent: NSEnumerationOptions

Specifies that the Block enumeration should be concurrent.

static var reverse: NSEnumerationOptions

Specifies that the enumeration should be performed in reverse.

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

struct NSSortOptions

Options for block sorting operations.

