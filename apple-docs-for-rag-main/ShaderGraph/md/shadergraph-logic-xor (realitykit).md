

- ShaderGraph
- Logic
-  XOR (RealityKit) 

ShaderGraph Node

# XOR (RealityKit)

Returns true if only one of the inputs is true.

## Parameter Types

| Input  | Type |
|--------|------|
| `In 1` | Bool |
| `In 2` | Bool |

| Output | Type |
|--------|------|
| `Out`  | Bool |

## Discussion

This node mimics the logical `Xor` operator. The table below shows the node’s output.

| In1   | In2   | Out   |
|-------|-------|-------|
| True  | True  | False |
| True  | False | True  |
| False | True  | True  |
| False | False | False |

## See Also

### Nodes

If Greater

Outputs True Result or False Result depending on whether value1 \> value2.

If Greater Or Equal

Outputs True Result or False Result depending on whether value1 \>= value2.

If Equal

Outputs True Result or False Result depending on whether value1 == value2.

Switch

Outputs the value from one of ten input streams, according to a selector .

And (RealityKit)

Boolean operation in1 && in2.

Or (RealityKit)

Boolean operation in1 \|\| in2.

Not (RealityKit)

Returns !input.

