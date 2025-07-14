

- GLKit
-  GLKMatrix3SetRow(\_:\_:\_:) 

Function

# GLKMatrix3SetRow(\_:\_:\_:)

Returns a new `3x3` matrix with one row replaced by a new vector.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3SetRow(
    _ matrix: GLKMatrix3,
    _ row: Int32,
    _ vector: GLKVector3
) -> GLKMatrix3
```

## Parameters 

`matrix`  

The source matrix.

`row`  

The index of the row to replace, which must be a number between `0` and `2`, inclusive.

`vector`  

A vector holding the replacement component values.

## Return Value

A new matrix.

## See Also

### Working With Parts of a Matrix

func GLKMatrix3GetMatrix2(GLKMatrix3) -> GLKMatrix2

Returns the upper-left `2x2` section of a `3x3` matrix.

func GLKMatrix3GetColumn(GLKMatrix3, Int32) -> GLKVector3

Retrieves a column from a `3x3` matrix.

func GLKMatrix3GetRow(GLKMatrix3, Int32) -> GLKVector3

Retrieves a row from a `3x3` matrix.

func GLKMatrix3SetColumn(GLKMatrix3, Int32, GLKVector3) -> GLKMatrix3

Returns a new `3x3` matrix with one column replaced by a new vector.

