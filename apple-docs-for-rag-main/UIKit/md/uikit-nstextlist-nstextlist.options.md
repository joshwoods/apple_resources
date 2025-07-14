

- UIKit
- NSTextList
-  NSTextList.Options 

Structure

# NSTextList.Options

Values that available options for text list items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Topics

### Options

static var prependEnclosingMarker: NSTextList.Options

Specifies that a nested list should include the marker for its enclosing superlist before its own marker.

### Initializers

init(rawValue: UInt)

Returns a new set of text list options using the raw value you specify.

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

### Getting list options

var isOrdered: Bool

var listOptions: NSTextList.Options

Returns the list options mask value of the receiver.

