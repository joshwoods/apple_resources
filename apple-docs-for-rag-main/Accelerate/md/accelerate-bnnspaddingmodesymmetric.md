

- Accelerate
-  BNNSPaddingModeSymmetric 

Global Variable

# BNNSPaddingModeSymmetric

A constant that indicates that a padding operation fills the padded area to form an even-symmetric pattern.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSPaddingModeSymmetric: BNNSPaddingMode { get }
```

## Discussion

For example, given the following padding size and input:

```
let paddingSize = (2, 4)

let source: [Float] = [ 0, 1, 2, 3, 4, 5, 7, 8, 9 ]

var destination = [Float](repeating: 0,
                          count: source.count + paddingSize.0 + paddingSize.1)
```

A padding operation using BNNSPaddingModeSymmetric populates destination with the following values:

```
[1.0, 0.0, 0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 7.0, 8.0, 9.0, 9.0, 8.0, 7.0, 5.0]
```

## See Also

### Padding Modes

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSPaddingModeConstant: BNNSPaddingMode

A constant that indicates that a padding operation fills the padded area with a specified constant.

var BNNSPaddingModeReflect: BNNSPaddingMode

A constant that indicates that a padding operation fills the padded area to form an odd-symmetric pattern.

