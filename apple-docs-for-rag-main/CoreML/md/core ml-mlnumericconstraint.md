

- Core ML
-  MLNumericConstraint 

Class

# MLNumericConstraint

The value limitations of a number.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 6.0+

``` source
class MLNumericConstraint
```

## Topics

### Numeric Constraints

var minNumber: NSNumber

The smallest numerical value allowed by this constraint.

var maxNumber: NSNumber

The largest numerical value allowed by this constraint.

var enumeratedNumbers: Set&lt;NSNumber>?

A set of the numbers allowed in this constraint.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Constraining Numeric Values

var numericConstraint: MLNumericConstraint?

The constraints of this paramter description value, if and only if the value is numerical.

