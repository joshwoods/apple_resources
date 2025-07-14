

- ShaderGraph
- Logic
-  If Greater 

ShaderGraph Node

# If Greater

Outputs True Result or False Result depending on whether value1 \> value2.

## Parameter Types

- If Greater (float)
- If Greater (color4f)
- If Greater (vector3f integer)
- If Greater (vector3f)
- If Greater (vector4f integer)
- If Greater (vector4h)
- If Greater (vector4f)
- If Greater (vector2h integer)
- If Greater (vector3h integer)
- If Greater (vector2f integer)
- If Greater (Float integer)
- If Greater (vector2h)
- If Greater (color3f)
- If Greater (half integer)
- If Greater (color3f integer)
- If Greater (color4f integer)
- If Greater (half)
- If Greater (vector2f)
- If Greater (vector4h integer)
- If Greater (vector3h)

| Input          | Type  |
|----------------|-------|
| `Value1`       | Float |
| `Value2`       | Float |
| `True Result`  | Float |
| `False Result` | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input          | Type   |
|----------------|--------|
| `Value1`       | Float  |
| `Value2`       | Float  |
| `True Result`  | Color4 |
| `False Result` | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Int32    |
| `Value2`       | Int32    |
| `True Result`  | Vector3f |
| `False Result` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Float    |
| `Value2`       | Float    |
| `True Result`  | Vector3f |
| `False Result` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Int32    |
| `Value2`       | Int32    |
| `True Result`  | Vector4f |
| `False Result` | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input    | Type     |
|----------|----------|
| `Value1` | Float    |
| `Value2` | Float    |
| `In 1`   | Vector4h |
| `In 2`   | Vector4h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Float    |
| `Value2`       | Float    |
| `True Result`  | Vector4f |
| `False Result` | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input    | Type     |
|----------|----------|
| `Value1` | Int32    |
| `Value2` | Int32    |
| `In 1`   | Vector2h |
| `In 2`   | Vector2h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input    | Type     |
|----------|----------|
| `Value1` | Int32    |
| `Value2` | Int32    |
| `In 1`   | Vector3h |
| `In 2`   | Vector3h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Int32    |
| `Value2`       | Int32    |
| `True Result`  | Vector2f |
| `False Result` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input          | Type  |
|----------------|-------|
| `Value1`       | Int32 |
| `Value2`       | Int32 |
| `True Result`  | Float |
| `False Result` | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input    | Type     |
|----------|----------|
| `Value1` | Float    |
| `Value2` | Float    |
| `In 1`   | Vector2h |
| `In 2`   | Vector2h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input          | Type   |
|----------------|--------|
| `Value1`       | Float  |
| `Value2`       | Float  |
| `True Result`  | Color3 |
| `False Result` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input    | Type  |
|----------|-------|
| `Value1` | Int32 |
| `Value2` | Int32 |
| `In 1`   | Half  |
| `In 2`   | Half  |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input          | Type   |
|----------------|--------|
| `Value1`       | Int32  |
| `Value2`       | Int32  |
| `True Result`  | Color3 |
| `False Result` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input          | Type   |
|----------------|--------|
| `Value1`       | Int32  |
| `Value2`       | Int32  |
| `True Result`  | Color4 |
| `False Result` | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input    | Type |
|----------|------|
| `Value1` | Half |
| `Value2` | Half |
| `In 1`   | Half |
| `In 2`   | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input          | Type     |
|----------------|----------|
| `Value1`       | Float    |
| `Value2`       | Float    |
| `True Result`  | Vector2f |
| `False Result` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input    | Type     |
|----------|----------|
| `Value1` | Int32    |
| `Value2` | Int32    |
| `In 1`   | Vector4h |
| `In 2`   | Vector4h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input    | Type     |
|----------|----------|
| `Value1` | Float    |
| `Value2` | Float    |
| `In 1`   | Vector3h |
| `In 2`   | Vector3h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

## Parameter descriptions

`Value1`  
The first value to compare.

`Value2`  
The second value to compare.

`True Result`  
The output of the node if the `Value1` input parameter is greater than the `Value2` input parameter.

`False Result`  
The output of the node if the `Value1` input parameter isn’t greater than the `Value2` input parameter.

## See Also

### Nodes

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

XOR (RealityKit)

Returns true if only one of the inputs is true.

Not (RealityKit)

Returns !input.

