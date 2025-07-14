

- GLKit
-  GLKMatrix4SetColumn(\_:\_:\_:) 

Function

# GLKMatrix4SetColumn(\_:\_:\_:)

Returns a new `4x4` matrix with one column replaced by a new vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix4SetColumn(
    _ matrix: GLKMatrix4,
    _ column: Int32,
    _ vector: GLKVector4
) -> GLKMatrix4
```

## Parameters 

`matrix`  

The source matrix.

`column`  

The index of the column to replace, which must be a number between `0` and `3`, inclusive.

`vector`  

A vector holding the replacement component values.

## Return Value

A new matrix.

## Discussion

The first three components of column `3` provide the translation values `tx`, `ty` and `tz`.

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

func GLKMatrix4SetRow(GLKMatrix4, Int32, GLKVector4) -> GLKMatrix4

Returns a new `4x4` matrix with one row replaced by a new vector.

