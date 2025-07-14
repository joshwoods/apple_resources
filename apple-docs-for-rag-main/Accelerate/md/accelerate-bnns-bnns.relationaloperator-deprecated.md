

- Accelerate
- BNNS
-  BNNS.RelationalOperator Deprecated

Structure

# BNNS.RelationalOperator

Constants that describe relational operations.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@frozen
struct RelationalOperator
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Relational Operators

static var equal: BNNS.RelationalOperator

The operator that indicates the equal-to relationship.

static var greater: BNNS.RelationalOperator

The operator that indicates the greater-than relationship.

static var greaterEqual: BNNS.RelationalOperator

The operator that indicates the greater-than or equal-to relationship.

static var less: BNNS.RelationalOperator

The operator that indicates the less-than relationship.

static var lessEqual: BNNS.RelationalOperator

The operator that indicates the less-than or equal-to relationship.

static var notEqual: BNNS.RelationalOperator

The operator that indicates the not-equal relationship.

### Logical Operators

static var and: BNNS.RelationalOperator

The operator that indicates the logical AND relationship.

static var nand: BNNS.RelationalOperator

The operator that indicates the logical NAND relationship.

static var nor: BNNS.RelationalOperator

The operator that indicates the logical NOR relationship.

static var not: BNNS.RelationalOperator

The operator that indicates the logical NOT relationship.

static var or: BNNS.RelationalOperator

The operator that indicates the logical OR relationship.

static var xor: BNNS.RelationalOperator

The operator that indicates the logical XOR relationship.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Sendable

