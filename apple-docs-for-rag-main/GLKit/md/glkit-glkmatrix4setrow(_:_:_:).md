

- GLKit
-  GLKMatrix4SetRow(\_:\_:\_:) 

Function

# GLKMatrix4SetRow(\_:\_:\_:)

Returns a new `4x4` matrix with one row replaced by a new vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4SetRow(
    _ matrix: GLKMatrix4,
    _ row: Int32,
    _ vector: GLKVector4
) -> GLKMatrix4
```

## Parameters 

`matrix`  

The source matrix.

`row`  

The index of the row to replace, which must be a number between `0` and `3`, inclusive.

`vector`  

A vector holding the replacement component values.

## Return Value

A new matrix.

## Discussion

The last component of rows `0` through `2` correspond to the translation values `tx`, `ty`, and `tz`, respectively.

## See Also

### Working With Parts of a Matrix

func GLKMatrix4GetMatrix2(GLKMatrix4) -> GLKMatrix2

Returns the upper-left `2x2` section of a `4x4` matrix.

func GLKMatrix4GetMatrix3(GLKMatrix4) -> GLKMatrix3

Returns the upper-left `3x3` section of a `4x4` matrix.

func GLKMatrix4GetColumn(GLKMatrix4, Int32) -> GLKVector4

Retrieves a column from a `4x4` matrix.

func GLKMatrix4GetRow(GLKMatrix4, Int32) -> GLKVector4

Retrieves a row from a `4x4` matrix.

func GLKMatrix4SetColumn(GLKMatrix4, Int32, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix with one column replaced by a new vector.

