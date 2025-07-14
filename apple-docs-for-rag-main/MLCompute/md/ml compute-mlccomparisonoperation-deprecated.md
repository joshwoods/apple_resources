

- ML Compute
-  MLCComparisonOperation Deprecated

Enumeration

# MLCComparisonOperation

A comparison operation.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
enum MLCComparisonOperation
```

## Topics

### Enumeration Cases

case equal

case greater

case greaterOrEqual

case less

case lessOrEqual

case logicalAND

case logicalNAND

case logicalNOR

case logicalNOT

case logicalOR

case logicalXOR

case notEqual

var debugDescription: String

A textual description of the comparison operation, suitable for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Comparison Layers

convenience init(operation: MLCComparisonOperation)

Creates a comparison layer with the operation you specify.

Deprecated

