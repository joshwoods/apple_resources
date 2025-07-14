

- GLKit
-  GLKMatrix3GetColumn(\_:\_:) 

Function

# GLKMatrix3GetColumn(\_:\_:)

Retrieves a column from a `3x3` matrix.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMatrix3GetColumn(
    _ matrix: GLKMatrix3,
    _ column: Int32
) -> GLKVector3
```

## Parameters 

`matrix`  

A `3x3` matrix.

`column`  

The column index, which must be a number between `0` and `2`, inclusive.

## Return Value

A vector representing the column retrieved from the matrix.

## See Also

### Working With Parts of a Matrix

func GLKMatrix3GetMatrix2(GLKMatrix3) -> GLKMatrix2

Returns the upper-left `2x2` section of a `3x3` matrix.

func GLKMatrix3GetRow(GLKMatrix3, Int32) -> GLKVector3

Retrieves a row from a `3x3` matrix.

func GLKMatrix3SetColumn(GLKMatrix3, Int32, GLKVector3) -> GLKMatrix3

Returns a new `3x3` matrix with one column replaced by a new vector.

func GLKMatrix3SetRow(GLKMatrix3, Int32, GLKVector3) -> GLKMatrix3

Returns a new `3x3` matrix with one row replaced by a new vector.

