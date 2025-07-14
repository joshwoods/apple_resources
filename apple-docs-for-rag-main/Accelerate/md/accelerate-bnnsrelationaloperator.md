

- Accelerate
-  BNNSRelationalOperator 

Structure

# BNNSRelationalOperator

Constants that describe relational operations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSRelationalOperator
```

## Topics

### Relational Operators

var BNNSRelationalOperatorEqual: BNNSRelationalOperator

The operator that indicates the equal-to relationship.

var BNNSRelationalOperatorGreater: BNNSRelationalOperator

The operator that indicates the greater-than relationship.

var BNNSRelationalOperatorGreaterEqual: BNNSRelationalOperator

The operator that indicates the greater-than or equal-to relationship.

var BNNSRelationalOperatorLess: BNNSRelationalOperator

The operator that indicates the less-than relationship.

var BNNSRelationalOperatorLessEqual: BNNSRelationalOperator

The operator that indicates the less-than or equal-to relationship.

var BNNSRelationalOperatorNotEqual: BNNSRelationalOperator

The operator that indicates the not-equal relationship.

### Logical Operators

var BNNSRelationalOperatorLogicalAND: BNNSRelationalOperator

The operator that indicates the logical AND relationship.

var BNNSRelationalOperatorLogicalNAND: BNNSRelationalOperator

The operator that indicates the logical NAND relationship.

var BNNSRelationalOperatorLogicalNOR: BNNSRelationalOperator

The operator that indicates the logical NOR relationship.

var BNNSRelationalOperatorLogicalNOT: BNNSRelationalOperator

The operator that indicates the logical NOT relationship.

var BNNSRelationalOperatorLogicalOR: BNNSRelationalOperator

The operator that indicates the logical OR relationship.

var BNNSRelationalOperatorLogicalXOR: BNNSRelationalOperator

The operator that indicates the logical XOR relationship.

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Tensor comparison layers

static func compare(BNNSNDArrayDescriptor, BNNSNDArrayDescriptor, using: BNNS.RelationalOperator, output: BNNSNDArrayDescriptor) throws

Performs an elementwise comparison of two array descriptors using the specified relational operator.

Deprecated

func BNNSCompareTensor(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSRelationalOperator, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>) -> Int32

Returns a tensor of Boolean type by comparing or performing a logical operation between two inputs.

Deprecated

