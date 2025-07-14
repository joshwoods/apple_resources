

- GLKit
-  GLKMathUnproject(\_:\_:\_:\_:\_:) 

Function

# GLKMathUnproject(\_:\_:\_:\_:\_:)

Projects a point in view space into object space.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func GLKMathUnproject(
    _ window: GLKVector3,
    _ model: GLKMatrix4,
    _ projection: GLKMatrix4,
    _ viewport: UnsafeMutablePointer,
    _ success: UnsafeMutablePointer?
) -> GLKVector3
```

## Parameters 

`window`  

The point in window coordinates.

`model`  

A modelview transformation matrix.

`projection`  

A projection matrix.

`viewport`  

A pointer to an array of four integer values. The first pair of values represent the window coordinates of the viewport’s bottom left corner. The second pair of values represent the width and height of the view port.

`success`  

Upon return, contains true if the function completed successfully, otherwise it contains false. Pass `NULL` if you do not want error information.

## Return Value

The projected point in object space.

## See Also

### Projecting Vectors

func GLKMathProject(GLKVector3, GLKMatrix4, GLKMatrix4, UnsafeMutablePointer&lt;Int32>) -> GLKVector3

Projects a point in object space into the window coordinate system.

